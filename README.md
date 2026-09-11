# 🛸 AEROSAVE: AI-Powered Autonomous Search & Rescue Drone

![SIH 2026](https://img.shields.io/badge/SIH-2026_Hardware-red?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)
![Stack](https://img.shields.io/badge/Stack-React_18_%7C_Tailwind_%7C_Leaflet-emerald?style=for-the-badge)
![AI Model](https://img.shields.io/badge/AI-YOLOv8_Vision-amber?style=for-the-badge)

> **Smart India Hackathon (SIH) 2026 Project**  
> An autonomous emergency disaster response drone and ground command dashboard designed for flood, earthquake, and landslide rescue operations.

---

## 🌐 Live Demo & Interactive Dashboard

🔗 **[Click Here to Launch Live AEROSAVE Command Center](https://kumariraunak-creator.github.io/aerosave-rescue-dashboard/aerosave.html)**

---

## 🎯 Problem Statement & Solution

During natural disasters (floods, earthquakes, building collapses), traditional rescue operations are delayed due to submerged roads and unsafe terrain. 

**AEROSAVE** solves this by combining aerial AI vision with autonomous hardware payload mechanics:
1. **Scans Disaster Zones**: Flies autonomous search grids over disaster areas.
2. **Detects Trapped Victims**: Uses real-time YOLOv8 computer vision to locate human victims.
3. **Delivers First-Aid**: Activates a Pixhawk-connected PWM servo mechanism to drop life-saving medical supplies.
4. **Broadcasts Voice Intercom**: Speaks automated Hindi/English messages (*"Madad aa rahi hai!"*) and listens for cries for help.
5. **Real-Time Telemetry**: Streams GPS coordinates, flight metrics, and victim locations to the Rescue Command Center.

---

## 🚀 Key Features

- **🚁 Live OpenStreetMap Command Center**: Interactive dark-themed Leaflet map showing drone position, search grid, hazard polygons (flood/fire/unsafe zones), and victim pins.
- **🧠 Real-Time YOLOv8 AI Stream**: Visual bounding boxes, confidence score rating (96%+), heatmap overlays, and target geo-tagging.
- **📦 First-Aid Servo Drop Mechanism**: Visualized servo arm rotation (0° ➔ 90°) for payload deployment.
- **📢 Voice Assistance & Audio Intercom**: Dual Hindi/English audio broadcast with dynamic acoustic equalizer waveform.
- **⚡ 1-Click SIH Judge Demo Mode**: Step-by-step automated workflow demonstrating complete disaster search & rescue cycle.

---


## 🛠️ System Architecture


---

## ⚙️ Hardware Bill of Materials (BOM)

| Component | Specification | Function |
| :--- | :--- | :--- |
| **Drone Frame** | F450 Quadcopter Frame | Rigid carbon/nylon structure |
| **Flight Controller** | Pixhawk 2.4.8 (PX4 / ArduPilot) | Autopilot navigation & PWM servo control |
| **AI Companion** | Android SBC / Companion Phone | Runs YOLOv8 inference locally |
| **Camera** | 1080p HD Wide-Angle Lens | Real-time aerial video feed |
| **GPS Module** | U-Blox Neo-M8N Dual Compass | 3D satellite positioning |
| **Drop Mechanism** | High-Torque PWM Servo | First-Aid payload release arm |
| **Radio Telemetry** | 433MHz 3DR Transceiver Pair | Long-range offline telemetry stream |
| **Power System** | 4S 5200mAh 35C LiPo Battery | Flight endurance & system power |

---

## 💻 Software & Tech Stack

- **Frontend Dashboard**: React 18, Tailwind CSS, Lucide Icons
- **Mapping & GIS**: Leaflet.js, OpenStreetMap, CARTO Dark Tiles
- **Computer Vision**: YOLOv8 Neural Network
- **Flight Software**: PX4 Autopilot Stack / MAVLink v2.0
- **Audio Processing**: Web Audio API & Acoustic Wave Visualizer

---

## 📥 Quick Local Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/kumariraunak-creator/aerosave-rescue-dashboard.git
   
