# Real-Time Energy Monitoring System

## Overview

The **Real-Time Energy Monitoring System** is a full-stack solution designed to track, analyze, and visualize energy consumption in real-time. Built using **Django, React.js, PostgreSQL, and Raspberry Pi**, this system enables users to **monitor voltage, current, and power usage** across multiple circuits, ensuring **energy efficiency, cost savings, and system reliability**.

Originally developed as part of a **home automation and sustainability initiative**, this system integrates **hardware sensors with software analytics** to provide actionable insights into energy usage patterns. The project was initiated after adding a **100-amp service panel** in the garage, which services **over a dozen circuits** across the house and property.

---

## **Electrical System & Infrastructure Upgrades**
✔ **100-Amp Electrical Subpanel** – Installed to support expanded electrical capacity.  
✔ **220V Electric Car Charger** – Dedicated circuit for **Tesla charging station**.  
✔ **8x 20A GFCI Circuits** – Providing power to **sump pumps, outdoor receptacles, and garage**.  
✔ **Multiple Sump Pump Installations** – Replaced and upgraded **two sump pumps**, including a **10-foot deep well pump**.  
✔ **Underground PVC Drainage System** – Dug a **20-foot trench** for routing water drainage.  
✔ **High-Quality Wiring Materials** – Utilized **Romex 12/2, 12/3, and 12/2 UFB wiring** with appropriate conduit.  
✔ **Multiple Junction Boxes** – Installed for proper load distribution and ease of maintenance.  
✔ **Circuit Monitoring System** – Integrated **Raspberry Pi with ADS1115 modules** for **analog-to-digital conversion of voltage and current data**.  
✔ **WiFi-Based Data Transmission** – Sends **real-time sensor data** to a **cloud-hosted PostgreSQL database** for storage and analysis.  

This extensive electrical work saved an estimated **$10,000-$20,000** in contractor costs and ensured a **code-compliant and scalable power system** for the property.

---

## **Key Features**
✔ **Live Data Tracking** – Monitor voltage, current, and power in real-time.  
✔ **Django Backend** – Handles data collection, storage, and API services.  
✔ **React.js Frontend** – Provides interactive dashboards for data visualization.  
✔ **PostgreSQL Database** – Ensures structured and scalable data management.  
✔ **Raspberry Pi Integration** – Captures sensor data from energy monitoring hardware.  
✔ **ADS1115 Modules for Analog-to-Digital Conversion** – Converts **voltage and current readings** from sensors into digital data.  
✔ **WiFi-Enabled Data Transmission** – Sensor data is **sent wirelessly** to a **cloud database** for real-time monitoring.  
✔ **Graphical Analytics** – Generates real-time and historical energy usage trends.  
✔ **Alert System** – Detects anomalies and sends notifications for irregular power usage.  
✔ **Historical Reporting** – Enables users to analyze past energy consumption patterns.  
✔ **Mobile-Friendly UI** – Accessible via web and mobile devices for remote monitoring.  
✔ **Secure Authentication** – User login and role-based access control for data protection.

---

## **Technical Architecture**
- **Frontend:** React.js + Chart.js for real-time data visualization.  
- **Backend:** Django REST Framework for API and data handling.  
- **Database:** PostgreSQL with optimized queries for efficient energy data retrieval.  
- **Hardware:** Raspberry Pi + ADS1115 modules for analog-to-digital conversion of circuit data.  
- **Communication:** WiFi-based data transmission to cloud-hosted PostgreSQL database.  
- **Processing:** Real-time updates using WebSockets between backend and frontend.

---

## **System Setup & Installation**
### **1️⃣ Hardware Setup**
- Connect **current and voltage sensors** to the **ADS1115 modules** on the **Raspberry Pi GPIO**.
- Configure the **Raspberry Pi to send data via WiFi** to the cloud database.
- Install **necessary drivers and libraries** for data acquisition.

### **2️⃣ Software Setup**
1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-username/real-time-energy-monitoring.git
   cd real-time-energy-monitoring
   ```
2. **Backend Setup (Django & PostgreSQL)**
   ```sh
   pip install -r requirements.txt
   python manage.py migrate
   python manage.py runserver
   ```
3. **Frontend Setup (React.js)**
   ```sh
   cd frontend
   npm install
   npm start
   ```
4. **Deploy & Monitor:**
   - Ensure **Raspberry Pi is collecting and transmitting sensor data**.
   - Use the **frontend dashboard to monitor and analyze energy usage in real-time**.

---

## **Use Cases**
- **Home Energy Optimization:** Track and reduce unnecessary energy consumption.
- **Industrial Power Monitoring:** Identify inefficiencies in manufacturing power usage.
- **Smart Grid Applications:** Enhance grid stability with real-time data analytics.
- **Solar Power Systems:** Monitor solar generation and grid reliance.

---

## **Future Enhancements**
- **AI-based Predictive Analytics** for energy forecasting.
- **IoT Connectivity** for integrating with smart home automation.
- **Cloud Data Storage & Remote Access** for enhanced availability.
- **Customizable User Alerts & Reports** for better energy management.

---

## **Intellectual Property & Usage Disclaimer**
This project and all associated documentation are the **intellectual property of Samuel Alaskewicz**. **All Rights Reserved.**  
Unauthorized reproduction, distribution, modification, or commercial use of any part of this work is strictly **prohibited** without explicit **written consent** from the owner.  
Any attempt to claim ownership, sell, or redistribute any portion of this project may result in legal action.

---

## **Contributors**
**Samuel Alaskewicz** - Lead Developer, Systems Engineer  

📌 **GitHub Repository:** [https://github.com/sammysosoftware/Real-Time-Energy-Monitoring-System]


