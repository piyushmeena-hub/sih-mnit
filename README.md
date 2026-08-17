# 🚧 Smart Road Damage Detection System

A real-time road monitoring and pothole detection system developed for **SIH @ MNIT Jaipur — Problem Statement #6**.

The system is designed to detect **potholes and road surface damage in real time** and automatically record their **location and severity**.

## 🎯 Problem Statement

> Develop a system that detects potholes and road surface damage in real time and automatically records their location and severity.

**Category:** Hardware
**Theme:** Smart Vehicles

## 💡 Proposed Solution

Our system uses a simulated vehicle equipped with virtual sensors to continuously monitor road conditions.

The system combines:

* 📷 **RGB Camera** — detects potholes and visible road damage
* 📡 **LiDAR / Depth Sensor** — estimates road-surface depth and structure
* 🧭 **IMU** — detects vehicle vibration and sudden vertical movement
* 📍 **GPS** — records the geographical location of detected damage

Sensor data is processed in real time to identify road defects and estimate their severity.

### System Pipeline

```text
Virtual Vehicle
      │
      ├── RGB Camera
      ├── LiDAR / Depth Sensor
      ├── IMU
      └── GPS
             │
             ▼
       Sensor Data Fusion
             │
             ▼
      Road Damage Detection
             │
             ▼
      Severity Estimation
             │
             ▼
      Location Recording
             │
             ▼
       Live Dashboard
```

## 🚀 Key Features

* Real-time pothole detection
* Road-surface damage detection
* Pothole severity estimation
* Location recording
* Multi-sensor data fusion
* Simulated vehicle environment
* Live visualization of detected road damage
* Road-condition mapping
* Detection history and reporting

## 🖥️ Simulation

The project is being developed as a **simulation-based prototype**.

The simulated environment contains:

* A virtual vehicle
* Roads with different surface conditions
* Potholes and road defects
* Virtual sensors
* Real-time vehicle movement
* Road-damage detection
* Location tracking

The objective is to demonstrate how the proposed system would operate on a real vehicle while allowing the complete solution to be tested in a controlled environment.

## 🧠 Detection & Analysis

When the vehicle encounters a damaged section of road, the system analyzes the available sensor information.

A detected defect can be represented as:

```text
Road Damage Detected

Type: Pothole
Severity: High
Location: Recorded
Confidence: 94%
Status: Logged
```

The detected damage is then added to the road-condition database/map.

## 📊 Dashboard

The planned dashboard will provide real-time information such as:

* Vehicle position
* Current road condition
* Detected potholes
* Damage severity
* Detection confidence
* Number of detected defects
* Road-condition map
* Sensor information

## 🏗️ Project Architecture

```text
                  ┌─────────────────┐
                  │ Virtual Road    │
                  │ Environment     │
                  └────────┬────────┘
                           │
                           ▼
                  ┌─────────────────┐
                  │ Virtual Vehicle │
                  └────────┬────────┘
                           │
            ┌──────────────┼──────────────┐
            ▼              ▼              ▼
         Camera          LiDAR           IMU
            │              │              │
            └──────────────┼──────────────┘
                           │
                           ▼
                  ┌─────────────────┐
                  │ Sensor Fusion   │
                  └────────┬────────┘
                           │
                           ▼
                  ┌─────────────────┐
                  │ Damage Detection │
                  └────────┬────────┘
                           │
                  ┌────────┴────────┐
                  ▼                 ▼
           Severity Analysis   Location Data
                  │                 │
                  └────────┬────────┘
                           ▼
                  ┌─────────────────┐
                  │ Live Dashboard  │
                  └─────────────────┘
```

## 🛠️ Technology Stack

The exact technology stack is being finalized. The project is expected to involve:

* **Robotics Simulation**
* **Computer Vision**
* **Sensor Fusion**
* **Python / C++**
* **ROS 2**
* **3D Simulation**
* **Mapping & Visualization**

## 📁 Project Structure

```text
sih-ps6-pothole-detection/
│
├── README.md
├── simulation/
├── perception/
├── sensors/
├── detection/
├── dashboard/
├── mapping/
├── docs/
└── tests/
```

## 🎯 Objectives

1. Detect potholes and road-surface damage in real time.
2. Estimate the severity of detected damage.
3. Record the location of each detected defect.
4. Combine information from multiple sensors.
5. Visualize road conditions in real time.
6. Demonstrate the complete system through simulation.

## 🔮 Future Scope

The system can later be extended to:

* Real-world vehicle deployment
* Large-scale road-condition mapping
* Cloud-based road-damage databases
* Automatic municipal reporting
* Advanced road-defect classification
* Predictive road-maintenance analysis
* Integration with connected vehicles

## 👥 Team

**SIH @ MNIT Jaipur — Internal Hackathon**

**Problem Statement:** PS #6 — Real-Time Pothole & Road Surface Damage Detection

---

> **Note:** This repository contains a prototype developed for the internal hackathon at MNIT Jaipur. The uploaded problem-statement document identifies these problems as sample statements for the internal hackathon and explicitly states that they are not the official SIH 2026 problem statements.
