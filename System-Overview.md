# SYSTEM OVERVIEW

## Purpose

This document provides an overview of the home electrical monitoring and automation system, detailing its components, functionality, and benefits.

## Project Goals

- **Real-time energy monitoring** of key electrical circuits
- **Automation and optimization** of power usage
- **Remote data access and visualization**
- **Enhanced safety and reliability** by tracking circuit performance

## Key Components

### **1. Electrical Subpanel & Circuits**

- 100A subpanel with multiple breakers
- Dedicated circuits for **garage lighting, sump pumps, and outdoor receptacles**
- 60A 2-pole breaker for **EV charger**

### **2. Monitoring & Control System**

- **Raspberry Pi** as the data collection hub
- **ADS1115 analog-to-digital converters** for current sensing
- **WiFi-based data transmission** to a cloud database

### **3. Software & Data Processing**

- **Django backend** for data processing and API access
- **React.js frontend** for live data visualization
- **PostgreSQL database** to store historical energy usage logs

## System Functionality

1. **Energy sensors track voltage and current** in key circuits
2. **Raspberry Pi processes data and transmits it to the cloud**
3. **User dashboard visualizes real-time power consumption**
4. **Alerts & notifications** can be set for unusual activity

## Expected Benefits

- **Cost savings** by identifying inefficient energy use
- **Remote monitoring** for sump pumps and critical circuits
- **Scalability** for additional sensors and automation features
- **Enhanced reliability** through proactive issue detection

## Conclusion

This system provides a **scalable and efficient energy monitoring solution**, combining electrical engineering with modern IoT and software technologies. Future upgrades may include **solar energy integration, AI-based anomaly detection, and home automation features.**

