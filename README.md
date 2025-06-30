# Flux-Code-Cubicle
# 🚍 IoT-Based Real-Time Bus Tracking System

## 🔷 Track: Omnidimension  
### 📌 Problem Statement: Public Transit & Fleet Scheduling – Code Cubicle 4.0
---

## 📌 Table of Contents
- [Problem Overview](#problem-overview)
- [Solution Architecture](#solution-architecture)
- [Tech Stack](#tech-stack)
- [Setup Instructions](#setup-instructions)
- [Demo Video](#demo-video)
- [Future Scope](#future-scope)
- [Team Members](#team-members)
- [Contributing](#contributing)
- [License](#license)

---

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

## 🚀 Solution Architecture

```plaintext
+-------------------+         +--------------------+         +-------------------+
|  GPS + Arduino    | --MQTT-->  Azure IoT Hub     | -->Kafka--> Node.js Server |
| + SIM800L GSM     |         | (MQTT endpoint)    |         |   (Kafka Consumer)|
+-------------------+         +--------------------+         +-------------------+
                                                                   |
                                                                   v
                                                          +------------------+
                                                          |  Next.js Frontend|
                                                          | (Live Map + UI)  |
                                                          +------------------+




## 👨‍💻 Team Members

We are a team of four passionate tech enthusiasts who collaborated to design, build, and deploy a fully functional IoT-based bus tracking system in real time.

| Name               | Role                         | Contribution Highlights                                  |
|--------------------|------------------------------|-----------------------------------------------------------|
| **Subhadip Paul**  | Backend & Hardware Engineer  | Led Arduino programming, SIM800L configuration, Azure IoT Hub integration, and Node.js Kafka backend |
| **Sumit Tiwari**   | IoT & Device Communication   | Managed SIM800L + GPS wiring, MQTT setup, device-to-cloud messaging, and circuit stability |
| **Utsho Banerjee** | Frontend Developer           | Developed the real-time map UI using Next.js and Leaflet, integrated Socket.IO for live updates |
| **Sunetra Ghosh**  | Cloud & Data Pipeline Expert | Set up Azure IoT routing, Kafka streaming, and handled message brokering to ensure real-time data flow |

> 🛠️ We worked closely together through every phase: design, hardware setup, backend APIs, cloud setup, and frontend UI. Team collaboration, planning, and testing were key to achieving a reliable real-time system.
