# Drone Mission Simulation using Mission Planner

![License](https://img.shields.io/badge/Project-L%26T%20EduTech-blue)
![University](https://img.shields.io/badge/Institution-Christ%20University-red)
![Platform](https://img.shields.io/badge/Platform-ArduPilot%20Mission%20Planner-orange)

## 📌 Project Overview
This project involves the virtual testing and simulation of a drone mission using **Mission Planner** and **SITL (Software In The Loop)**. The goal was to configure a stable flight path, verify telemetry data, and ensure safety protocols (RTL) before physical deployment.

---

## 👥 Team Members
* **ALBIN MATHEW** - 2363007
* **AKILESH J K** - 2363006
* **ABDULLA MOHAMED ASHRAF** - 2363004
* **AADHITYA SAKTHIVEL REVATHY** - 2363002

---

## 📸 Mission Visuals

### 1. Pre-Flight Configuration
The initial setup showing the drone in a **DISARMED** state, confirming GPS Lock and EKF health before takeoff.
![Initial Setup](Screenshots/Screenshot_171319.jpg)

### 2. Waypoint Navigation
The drone actively following the planned path at a ground speed of **10 m/s**.
![Mission Path](Screenshots/Screenshot_171444.jpg)

### 3. Telemetry & Flight Data
Real-time monitoring of altitude (21m) and heading alignment during the simulation.
![Telemetry Data](Screenshots/Screenshot_171515.jpg)

---

## ⚙️ Technical Specifications
* **Firmware:** ArduCopter V4.6.0-dev (Quadcopter)
* **Ground Speed:** 10 m/s
* **Target Altitude:** 21 m
* **GPS Status:** 3D Fix / RTK Fixed
* **Simulation Environment:** SITL (Software In The Loop)

---

## 🗺️ Mission Architecture
1. **Takeoff:** Vertical climb to 21 meters.
2. **Waypoint Navigation:** A 4-point perimeter circuit (Waypoints 1-4).
3. **Telemetry Monitoring:** Real-time tracking of ground speed and EKF health.
4. **RTL (Return to Launch):** Automated landing at the Home position upon completion.

---

## 📂 Repository Structure
```text
├── MissionFiles/
│   └── mission_plan.waypoints   # GPS Waypoint file
├── Config/
│   └── drone_params.param       # Drone tuning & speed settings
├── Logs/
│   └── flight_telemetry.tlog    # Flight data recording
├── Screenshots/                 # Visual proof of simulation (Add your .jpg files here)
└── README.md                    # Project documentation
