# ENERGY DATA LOGGING & ANALYSIS

## Purpose
This document details how energy data is collected, logged, and analyzed to improve efficiency and detect abnormalities in the electrical monitoring system.

## Data Collection Process
1. **Current & Voltage Sensing**:
   - SCT-013-000 sensors measure current flow on monitored circuits.
   - ADS1115 ADC modules convert analog signals for Raspberry Pi processing.
   - Voltage readings are sampled using reference sensors.
2. **Raspberry Pi Processing**:
   - Reads real-time data from sensors every **5 seconds**.
   - Sends processed values to a **PostgreSQL database**.
3. **Data Transmission & Storage**:
   - WiFi module (ESP8266) transmits logs to the cloud database.
   - Historical data stored for analysis and visualization.

## Data Metrics Captured
| **Metric** | **Unit** | **Description** |
|-----------|---------|----------------|
| Current Load | Amperes (A) | Measures current draw per circuit |
| Voltage | Volts (V) | Tracks supply voltage levels |
| Power Consumption | Watts (W) | Real-time energy usage |
| Energy Usage | Kilowatt-hours (kWh) | Accumulated energy consumption |
| Anomalies | Events | Detects spikes, dropouts, and inefficiencies |

## Analysis & Insights
### **1. Real-Time Power Monitoring**
- Dashboard displays power usage **by circuit**.
- Enables **immediate response** to faults or anomalies.

### **2. Historical Trend Analysis**
- Logs energy consumption over **days, weeks, and months**.
- Identifies **inefficient power usage patterns**.

### **3. Alerts & Notifications**
- Automatic alerts for **overloads or unexpected spikes**.
- Sends notifications via **email or SMS** if predefined thresholds are exceeded.

## Example Data Snapshot
```json
{
    "timestamp": "2024-11-10 14:30:00",
    "circuit": "Sump Pump 1",
    "current": 3.5,
    "voltage": 120.5,
    "power": 420,
    "energy_usage": 0.35,
    "surge_power": 1260
}
```

## Future Enhancements
- **AI-based predictive maintenance** for early fault detection.
- **Machine learning models** to optimize energy consumption.
- **Solar energy integration** for alternative power tracking.

## Conclusion
The energy monitoring system provides valuable real-time insights, enabling **smarter energy management**, **fault detection**, and **cost savings**. Regular analysis helps improve **efficiency and safety** while allowing for future scalability.

