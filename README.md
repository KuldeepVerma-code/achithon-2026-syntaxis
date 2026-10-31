# Hackathon Problem-Solving Workspace — Team Nova Minds

**Selected Problem Statement:** PS10 – Open Innovation: Hardware / Embedded Systems / IoT Solution  
**Project Title:** Smart Real-Time Water Quality Monitoring System

---

## Project Overview

This repository contains the official solution developed by Team Nova Minds for Achithon 2026. 

Water contamination is a critical environmental and public health issue. Traditional manual testing methods are slow, labor-intensive, and fail to provide immediate alerts during sudden contamination events. 

Our project resolves this challenge by introducing an IoT-enabled, real-time water quality monitoring solution. Powered by an ESP32 microcontroller, the system continuously monitors key physical and chemical parameters of water, displays live telemetry locally on an integrated TFT display, triggers physical safety alarms during critical threshold breaches, and streams real-time data to a web dashboard via Firebase.

---

## Selected Challenge Specification

* **Problem Statement ID:** PS10
* **Category:** Open Innovation (Hardware / Embedded Systems / IoT Solution)
* **Core Focus:** Real-Time Data Acquisition, Signal Processing, Edge Alarm Logic, and Web Interface Integration.

---

## Key Technical Features

### Continuous Telemetry Sampling
The system performs high-frequency continuous data acquisition from connected water sensors using the ESP32 processing core.

### On-Device Hardware Monitoring
Includes a local TFT LCD screen to display real-time parameter values directly at the hardware deployment site without relying on active internet access.

### Dual-Layer Edge & Remote Alarm Logic
If sensor parameters cross predefined safety limits, the system triggers immediate local hardware actions (activating relays, sounding a buzzer, and toggling status LEDs) while simultaneously updating cloud data tags.

### Cloud Integration & Live Web Dashboard
Data is synced instantaneously to Firebase Realtime Database. Users and evaluators can monitor telemetry updates remotely using the interactive web dashboard (`index.html`) accessible from any browser.

---

## Technical Stack & Hardware Architecture

### Hardware Components
* **Microcontroller:** ESP32 Development Board (Integrated Wi-Fi Module)
* **Display Interface:** TFT LCD Module
* **Output & Actuators:** 2-Channel Relay Module, Active Piezoelectric Buzzer, Indicator LEDs
* **Prototyping Setup:** Breadboard, Jumper Interconnects, External Power Source

### Software Architecture
* **Firmware:** C++ / Embedded C compiled via Arduino IDE (`arduinoidecode.ino`)[span_2](start_span)[span_2](end_span)
* **Cloud Infrastructure:** Firebase Realtime Database
* **Web Frontend:** Interactive Dashboard (`index.html`)[span_3](start_span)[span_3](end_span)

---

## Repository Structure

```text
├── arduinoidecode.ino    # ESP32 firmware source code
├── index.html            # Real-time Web Monitoring Dashboard
├── TEAM NOVA MINDS.pdf   # Team documentation & project report[PPT]
├── PS10.md               # Selected problem statement documentation
└── README.md             # Main project documentation file
