# 🌐 IoT Summer School Internship 2026 — Week 4

Welcome to the **Week 4** repository of the **IoT Summer School Internship 2026**. This module focuses on end-to-end IoT system development using the **ESP32** microcontroller, environmental data acquisition via sensors, REST API integration, and comparative analysis of IoT application layer protocols.

---

## 📋 Table of Contents
- [Overview](#-overview)
- [Projects & Assignments](#-projects--assignments)
  - [1. ESP32 Weather Data Fetcher & DHT11 Interfacing](#1-esp32-weather-data-fetcher--dht11-interfacing)
  - [2. IoT Protocol Evaluation: MQTT vs. HTTP](#2-iot-protocol-evaluation-mqtt-vs-http)
- [Hardware & Software Requirements](#-hardware--software-requirements)
- [Repository Structure](#-repository-structure)
- [Setup & Installation](#-setup--installation)
- [Security & Configuration](#-security--configuration)
- [Key Learning Outcomes](#-key-learning-outcomes)
- [Author & Submission Details](#-author--submission-details)

---

## 🎯 Overview
Week 4 bridges edge sensor interfacing with cloud connectivity. The core objectives involve reading local environmental metrics (temperature and humidity), fetching real-time meteorological data from external web services, and analyzing communication protocols for large-scale IoT deployments.

---

## 🚀 Projects & Assignments

### 1. ESP32 Weather Data Fetcher & DHT11 Interfacing
* **File:** `Question35_Weather_Data_Fetcher.ino`
* **Description:** An embedded application utilizing the ESP32 WiFi capabilities to interact with the **OpenWeatherMap REST API**. Simultaneously, the microcontroller interfaces with a local **DHT11 sensor** to read ambient temperature and humidity.
* **Key Features:**
  - Secure HTTPS/HTTP GET requests to fetch live JSON weather data.
  - JSON payload parsing using `ArduinoJson` to extract key parameters (temperature, humidity, weather conditions).
  - Local sensor data acquisition and comparison against cloud-reported metrics.

### 2. IoT Protocol Evaluation: MQTT vs. HTTP
* **Description:** A detailed architectural and performance comparison between **MQTT** (Message Queuing Telemetry Transport) and **HTTP** (Hypertext Transfer Protocol) in the context of IoT scalability.
* **Key Findings:**
  - Evaluated bandwidth consumption, packet overhead, latency, and power efficiency.
  - Concluded on the superiority of lightweight publish-subscribe architectures (MQTT) over request-response models (HTTP) for dense deployments (e.g., 1,000+ node smart agriculture networks).

---

## 🛠 Hardware & Software Requirements

### Hardware
* **Microcontroller:** ESP32 Development Board (e.g., NodeMCU-32S / ESP32-WROOM-32)
* **Sensor:** DHT11 or DHT22 Temperature & Humidity Sensor
* **Components:** 10kΩ Pull-up Resistor (if required for DHT data line), Breadboard, and Jumper Wires

### Software & Libraries
* **IDE:** Arduino IDE (v2.x recommended) or PlatformIO (VS Code)
* **Required Libraries:**
  - `WiFi.h` & `HTTPClient.h` (Built-in ESP32 core libraries)
  - `DHT sensor library` by Adafruit
  - `Adafruit Unified Sensor` by Adafruit
  - `ArduinoJson` by Benoit Blanchon (v6.x / v7.x)

---

## 📂 Repository Structure

```text
week4/
├── Question35_Weather_Data_Fetcher.ino   # Main ESP32 source code
├── config.example.h                      # Template for WiFi & API credentials
├── .gitignore                            # Security rules to prevent key leakage
├── Week4_Assignment_Report.pdf           # Comprehensive assignment report & protocol analysis
└── README.md                             # Project documentation (this file)
