# 🌿 AgriVision: Smart Plant Monitoring Dashboard

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Flask](https://img.shields.io/badge/Flask-Microservices-green)
![AI](https://img.shields.io/badge/AI-Gemini%20%2B%20MobileNetV2-orange)
![Database](https://img.shields.io/badge/Database-Firebase-yellow)

**A cloud-based IoT and AI ecosystem designed to bridge the physical garden with digital intelligence.**

---

## 📖 Overview

**AgriVision** is an innovative end-to-end platform that helps users track plant health in real-time. By combining live IoT sensor telemetry, Computer Vision, and Generative AI, the platform enables users to detect plant issues early, optimize growing conditions, and maintain a sustainable garden through gamified tasks.

The system simulates a distributed cloud environment using **Microservices architecture** within a notebook, ensuring robust data handling and AI orchestration.

---

## 🧠 Key Features

### 🌡️ Real-time IoT Sensor Monitoring
Track critical environmental metrics instantly to ensure optimal growth:
* **Temperature & Humidity:** Live tracking of ambient conditions.
* **Soil Moisture:** Alerts when watering is needed.
* **Light Intensity:** Monitoring sun exposure.

### 🤖 Hybrid AI Image Analysis
A dual-layer diagnostic pipeline:
1.  **Vision Layer (MobileNetV2):** Instantly classifies diseases (e.g., Leaf Spot, Water Stress) from uploaded images.
2.  **Reasoning Layer (Gemini AI):** Generates actionable, step-by-step treatment plans based on the diagnosis.

### 🔍 RAG-based Research Assistant
* **Retrieval-Augmented Generation (RAG):** A custom search engine that queries a curated database of academic plant-disease articles.
* Provides answers backed by scientific citations rather than generic LLM hallucinations.

### 📡 Microservices & Connectivity
* **IoT Gateway (Port 5001):** Simulates MQTT/REST communication to fetch and normalize sensor data.
* **AI Orchestrator (Port 5002):** Manages context, prompts, and GenAI interactions.

### 🎮 Gamification System
* **"Twin-Brain" Task Generation:** Creates daily missions based on both sensor data (e.g., "High heat detected -> Turn on fan") and plant health status.
* **XP & Leveling:** Users earn points and level up by completing sustainable farming tasks.

### 📊 Analytics & Dashboards
* **User Dashboard:** Personalized insights, active alerts, and "My Garden" history.
* **Admin/Analytics:** Visual charts (Matplotlib) showing historical trends of sensor data over time.

---

## 🛠️ Tech Stack

* **Language:** Python
* **Backend:** Flask (Multi-threaded Microservices)
* **AI & ML:** Google Gemini 2.5 Flash, MobileNetV2 (Transformers), Scikit-Learn (TF-IDF for RAG)
* **Database:** Firebase Realtime Database
* **Frontend:** IPython Widgets (Jupyter/Colab Integration)

---

## 👥 Contributors

This project was built with collaboration, dedication, and creativity by:

| Name | Role |
| :--- | :--- |
| **Lama Abu Abla** | System Architect & Gamification/Rewards Logic |
| **Shadi Alkeesh** | RAG Engine, Gemini Integration & Chatbot |
| **Safa Awad** | Automated Alert System & Health Logic |
| **Marwa Awad** | IoT Sensor Gateway & Big Data Analytics |

---

## 🎓 Acknowledgments

With the guidance and support of our lecturers:
* **Dr. Naomi Unkelos-Shpigel**
* **Nataly Levi**

---

### 🚀 How to Run
1.  Clone the repository.
2.  Add your `GOOGLE_API_KEY` and Firebase URL in the configuration cells.
3.  Run the notebook to initialize the Microservices (Ports 5001/5002).
4.  Launch the **AgriVision Cloud** interface.
