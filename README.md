# ⭐ Vertex AI Conversational Intelligence Platform  
### Multimodal Speech Understanding • Sentiment Detection • Serverless Deployment

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![Flask](https://img.shields.io/badge/Flask-Backend-black)
![Google Cloud](https://img.shields.io/badge/Google%20Cloud-Vertex%20AI-success)
![Cloud Run](https://img.shields.io/badge/Deployment-Cloud%20Run-orange)
![Architecture](https://img.shields.io/badge/Design-Cloud--Native-blueviolet)

---

## 🚀 Live Application

👉 **Launch App:**  
https://project3-610853696776.us-east1.run.app  

👉 **Cloud Run Metrics:**  
https://console.cloud.google.com/run/detail/us-east1/project3/metrics?project=convai-449103  

✅ Fully serverless deployment — no local setup required.

---

## 🧠 Executive Overview

This project implements a **cloud-native Conversational AI web application** powered by **Google Cloud Vertex AI Multimodal LLM** to extract insights directly from spoken language.

Users can upload or record audio, and the system returns:

- ✅ Speech transcription  
- ✅ Sentiment analysis  
- ✅ Downloadable results  

All outputs are saved using uniquely generated filenames to preserve historical interactions.

> The solution demonstrates how multimodal LLMs consolidate multiple NLP tasks into a **single high-efficiency API call**, significantly simplifying system architecture.

---

### Engineering Signals

- ✅ Multimodal LLM integration  
- ✅ Cloud-native deployment  
- ✅ Stateless backend  
- ✅ Timestamp-based storage  
- ✅ RESTful architecture  
- ✅ Automated artifact persistence  

These represent **production-level engineering decisions**.

---
---

## 🧠 Architecture Insight

The backend communicates with **Google Vertex AI Multimodal LLM** to process uploaded audio and generate both transcription and sentiment in a single request.  

Artifact storage ensures efficient file management, organized retrieval, and historical traceability of interactions.

This architecture minimizes API overhead while maximizing processing efficiency — a key principle in modern AI system design.

---

## ⚡ Core Features

### 🎙️ Real-Time Audio Recording
- Record audio directly from the browser  
- Live timer displays recording duration  
- Stop control prepares the file for AI processing  

---

### 📤 Audio Upload & Processing
- Automatically saves audio in `.wav` format  
- Sends audio to Vertex AI Multimodal LLM  
- Retrieves transcription and sentiment in a **single response**  

---

### 📂 Artifact Persistence
- Results saved as `.txt` files  
- Linked alongside original audio recordings  
- Timestamp-based naming prevents filename conflicts  

---

### 🔊 Audio Playback
- Built-in browser playback for recordings  
- Download links available for:
  - Original `.wav` audio  
  - Generated transcript  

---

### 🧠 AI-Powered Language Understanding

Vertex AI performs:

✔ Speech-to-text conversion  
✔ Sentiment classification  
✔ Context-aware language interpretation  

---

## ☁️ Cloud-Native Deployment

The application is deployed on **Google Cloud Run**, providing:

- Automatic scaling  
- Built-in load balancing  
- Fully managed infrastructure  
- High availability  

This ensures the system remains fast, responsive, and completely serverless.

---

## 🧰 Technology Stack

### 👨‍💻 Languages
- Python  
- JavaScript  
- HTML  

### ⚙️ Backend
- Flask REST API  
- GET / POST routing  
- Secure file handling  

### ☁️ Cloud & AI
- Google Vertex AI Multimodal LLM  
- Google Cloud Run  

### 💾 Storage
- Organized local file system  
- Timestamp-based artifact naming  

---

## 📂 Repository Structure

convai/
│
├── templates/
│ └── index.html
│
├── uploads/
├── main.py
├── script.js
├── requirements.txt
└── Dockerfile

---

This structure supports efficient routing, scalable API communication, and maintainable file management.

---

## ⚙️ Local Setup

### ✅ Requirements
- Python 3.10+
- Google Cloud Project
- Vertex AI enabled

---

### 🔐 Authenticate

**Mac/Linux**
```bash
export GOOGLE_APPLICATION_CREDENTIALS="path/to/service-account.json"

---

## 🏗️ High-Level Architecture

```mermaid
flowchart LR
    A[Client Browser] --> B[HTML + Flask UI]
    B --> C[Flask Backend]
    C --> D[Vertex AI Multimodal LLM]
    D --> E[Transcription + Sentiment]
    E --> F[Timestamped Storage]
    F --> G[Cloud Run Deployment]
