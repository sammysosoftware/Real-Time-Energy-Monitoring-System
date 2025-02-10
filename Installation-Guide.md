# INSTALLATION & SETUP GUIDE

## Purpose
This document provides step-by-step instructions for setting up the electrical monitoring and automation system, ensuring a safe and efficient installation process.

## Disclaimer
**WARNING:** This installation involves high-voltage electrical components and should only be performed by a **qualified and licensed electrician**. Improper handling of electrical systems can result in serious injury, death, or fire hazards. Always adhere to local electrical codes and regulations.

## Prerequisites
- **Professional electrical knowledge** and adherence to safety standards
- **Required tools**: Wire strippers, multimeter, screwdriver set, drill, electrical tape
- **Components from Bill of Materials**

## Step 1: Subpanel Installation
1. **Turn off main power** at the service panel.
2. Mount the **100A subpanel** securely near the main panel.
3. **Ensure proper mounting clearance**:
   - A minimum of **30 inches of workspace clearance** on both sides.
   - The panel must be installed at a height where the top breaker is no higher than **6 feet 7 inches** from the floor.
   - Ensure at least **3 feet of unobstructed workspace depth** in front of the panel.
4. Connect **4 AWG aluminum wire** from the main panel to the subpanel.
5. Install and label the **breakers** according to the wiring plan.

## Step 2: Wiring the Circuits
1. Run **12/2 Romex wire** from the panel to each circuit location.
2. Connect breakers:
   - 60A 2-pole → **Car charger**
   - 20A GFCI → **Garage lights & openers**
   - 20A GFCI → **Indoor outlets**
   - 4x 20A GFCI → **Outdoor sump pumps**
   - 4x 20A GFCI → **Outdoor outlets**
3. Use **junction boxes** where necessary and ensure **proper grounding**.

## Step 3: Installing the Monitoring System
1. Mount the **Raspberry Pi** in a secure, ventilated location (Junction box adjacent to electrical panel via conduit).
2. Connect **ADS1115 modules** to the Pi's GPIO.
3. Attach **current sensors (SCT-013-000) to hot lines** for monitoring.
4. Ensure the **WiFi module (ESP8266) is configured** for data transmission.

## Step 4: Software Installation
1. Install **Raspberry Pi OS** and update packages.
2. Install dependencies:
   ```bash
   sudo apt update && sudo apt install python3-pip
   pip install django requests numpy
   ```
3. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/energy-monitoring.git
   ```
4. Set up **PostgreSQL database** and run migrations.

## Step 5: System Testing & Validation
1. **Check wiring continuity** using a multimeter.
2. **Power on the panel** and monitor for faults.
3. **Verify Raspberry Pi data transmission** via the dashboard.
4. **Test circuit loads** to ensure safe operation.

## Safety Notes
- This installation must be performed by a **licensed electrician**.
- Always **follow electrical codes** and safety guidelines.
- Ensure **proper clearance and accessibility** to meet electrical code requirements.
- If unsure, consult a **certified electrical inspector** before proceeding.

## Conclusion
By following this guide, you will successfully set up an **energy monitoring and automation system** with a safe and structured approach. Future enhancements may include **solar integration and machine learning-based anomaly detection**.

