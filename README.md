# Flux-Code-Cubicle
# 🚍 IoT-Based Real-Time Bus Tracking System

## 🔷 Track: Omnidimension  
### 📌 Problem Statement: Public Transit & Fleet Scheduling – Code Cubicle 4.0

A smart, scalable, and cloud-connected IoT solution to enable real-time tracking of public buses using GPS, MQTT, Azure IoT Hub, Kafka, and web technologies.

---

## 🧠 Problem Overview

Urban commuters often suffer due to unreliable public transport systems with no visibility into real-time bus locations. This leads to time wastage, over-crowding, and operational inefficiencies.

### ✅ Our Goal:
To develop a system that enables **real-time bus tracking**, allowing both users and fleet operators to view and optimize bus movements via live maps and updates.

---

## 🚀 Solution Overview

We built a full-stack IoT solution that:
- Captures **real-time GPS data** from buses
- Transmits the data using **SIM800L + MQTT**
- Ingests it into **Azure IoT Hub**
- Streams it via **Apache Kafka**
- Delivers it to a **Next.js-based frontend** using **Socket.IO**

---

## 🔧 Tech Stack

### 🖥️ Hardware:
- Raspberry Pi
- Arduino (ATmega328P)
- Neo-6M GPS Module
- SIM800L GSM Module

### ☁️ Cloud and Messaging:
- Azure IoT Hub (MQTT protocol)
- Apache Kafka (real-time streaming)
- Node.js Backend
- Socket.IO

### 🌐 Frontend:
- Next.js (React)
- Leaflet.js (Map visualization)
- Socket.IO (Live updates)

---

## 🧭 System Architecture

```plaintext
GPS (Neo-6M) → Arduino → SIM800L → Azure IoT Hub (MQTT) → Kafka → Node.js Server → Socket.IO → Next.js Frontend (Map UI)
