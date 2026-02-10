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

## 🏗️ High-Level Architecture

```mermaid
flowchart LR
    A[Client Browser] --> B[HTML + Flask UI]
    B --> C[Flask Backend]
    C --> D[Vertex AI Multimodal LLM]
    D --> E[Transcription + Sentiment]
    E --> F[Timestamped Storage]
    F --> G[Cloud Run Deployment]
