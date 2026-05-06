# Jayasuryaa Chandrasekar

> **Project-driven AI Engineer** building intelligent, end-to-end ML systems with hands-on experience in temporal, behavioral, and performance-critical data — complemented by a full-stack development background.

**Pre-Final Year** | SRM Institute of Science and Technology (CGPA: 8.65/10)

---

## 📌 Quick Links
🔗 [**Portfolio**](https://jayasuryaa.vercel.app) • 📧 [jayasuryaa1785@outlook.com](mailto:jayasuryaa1785@outlook.com) • 💼 [LinkedIn](https://linkedin.com/in/jayasuryaachandrasekar/) • 🐙 [GitHub](https://github.com/pixelpitstop)

---

## 🚀 Featured Projects

### **⚡ Electricity Anomaly Detection System** — *Production-Grade ML*
[**Repository**](https://github.com/pixelpitstop/Time-Series-Forecasting)  
A production-oriented ML system for detecting anomalous electricity demand in the PJME hourly grid dataset. Forecast 24h ahead → compute residual → flag anomalies at calibrated thresholds — grounded in industrial monitoring practice.

**Key Engineering Features:**
- Configurable anomaly threshold via residual quantile (99th percentile default)
- Per-anomaly-type evaluation: spike, drop, flatline with detection delay tracking
- Drift handling: threshold recalibration + model retraining
- **Outputs:** detection_metrics.json, anomaly_type_metrics.csv, scored_test_window.csv

**Tech Stack:** Python, XGBoost, pandas, FastAPI, Streamlit, pytest, uvicorn  
**Architecture:** Raw Data → Feature Engineering → 24h XGBoost Forecast → Residual Engine → Threshold → Anomaly Flags → API/CLI

---

### **🚗 CANInsight — Vehicle Diagnostics & Telemetry Intelligence**
[**Repository**](https://github.com/pixelpitstop/Canbus-project) • [**Live App**](https://caninsight.streamlit.app)  
Complete automotive CAN bus diagnostics pipeline mimicking real vehicle ECU data handling — from raw bytes to operator-facing insights, built as a demo-ready product.

**5-Stage Pipeline:**
- **Parsing:** Raw CAN-like logs (timestamp + ID + hex) → structured byte arrays
- **Signal Extraction:** Bytes → engineering signals (RPM, throttle %, speed, engine temp, brake %)
- **Rule-Based Diagnostics:** Detects operational events (overheating, RPM spikes, harsh braking) with severity scoring
- **Insight Generation:** Raw alerts → human-readable summary with risk level, priorities, recommended actions
- **Streamlit Dashboard:** Telemetry charts, trip score, max readings, alerts table, insight report

**Tech Stack:** Python, Streamlit, pandas, structured event system  
**Modules:** decoder.py, analysis.py, insights.py, pipeline.py, dashboard.py, generate_can_data.py

---

### **🛡️ Smart Vehicle Diagnostics & Intrusion Detection System** — *In Progress*
[**Repository**](https://github.com/pixelpitstop/Smart-Vehicle-Diagnostics-Intrusion-Detection-System)  
Extended vehicle intelligence platform combining CANInsight diagnostics with CAN bus security and real-time intrusion detection. Designed to flag anomalous or injected CAN frames at the signal level using behavioral analysis.

**Focus:** Automotive cybersecurity, real-time telemetry, ECU-level attack vector detection (replay attacks, message injection, sensor spoofing)  
**Tech Stack:** Python  
**Status:** Active development

---

### **🏎️ F1 AI Telemetry Analyzer** — *In Progress*
[**Repository**](https://github.com/pixelpitstop/F1-AI-Telemetry-Analyzer)  
Physics-aware ML system analyzing **12GB+ of F1 telemetry data** from FastF1.  
**Key Results:** 97.8% accuracy, 0.49s lap-time MAE, corner-level performance insights  
**Tech:** FastF1, scikit-learn, pandas, numpy, matplotlib

---

### **🌍 Urban Thermal Equity Index (UTEI) — Chennai**
[**Repository**](https://github.com/pixelpitstop/Urban-Thermal-Equity-Index-using-Machine-Learning)  
Research-grade geospatial ML project introducing a novel metric to quantify heat distribution inequality across city neighborhoods. Built during MSSRF internship.

**UTEI Formula:** Land Surface Temperature (MODIS) + Humidity (IoT/weather) − Vegetation Index (Sentinel-2 NDVI)  
**Model:** Lasso regression trained on fused geospatial dataset  
**Outputs:**
- Per-location UTEI scores across Chennai (utei_predictions.csv)
- Ranked hotspot-to-coolest-zone list (utei_sorted.csv)
- Interactive Leaflet/Folium thermal equity heatmap (temperature_heatmap.html)

**Tech Stack:** Python, pandas, scikit-learn, Folium, Google Earth Engine, MODIS/Sentinel-2  
**Impact:** First index combining vegetation, land temperature, and humidity for measuring thermal equity

---

### **🚘 AutoIntel — AI Car Recommendation Engine** — *In Progress*
[**Repository**](https://github.com/pixelpitstop/Car-recommendation-project)  
Production-oriented car recommendation service combining structured vehicle catalog data with NLP-driven review intelligence for explainable, ranked recommendations.

**Architecture:**
- **Data Ingestion:** Normalized vehicle catalog collection
- **NLP Layer:** Sentiment extraction, pros/cons, common issues from owner reviews
- **Feature Engineering:** Text embeddings + structured feature vectors (price, specs, reliability)
- **Hybrid Scoring:** Weighs multiple signals for buyer profile tailoring

**API Endpoints:** POST /recommend, GET /cars, GET /health  
**Codebase:** ingestion/ → features/ → nlp/ → recommendation/ → evaluation/ → api/ → frontend/  
**Tech Stack:** Python, FastAPI, NLP embeddings, pandas, pytest

---

### **🤖 AI MUN Assistant — Local-First RAG Chatbot**
[**Repository**](https://github.com/pixelpitstop/AI-Chatbot-project)  
Production-grade AI assistant for Model United Nations delegates — demonstration of a complete, local-first RAG system with streaming, memory, and structured generation.

**Key Features:**
- Document ingestion → chunking & embedding → persistent vector index
- Redis-backed short-term memory (recent context)
- File-backed strategy memory (allies, opponents, position notes)
- Argument generation route (opening statements, counter-arguments, cross-questions)
- Server-Sent Events (SSE) streaming for low-latency UX

**Benchmarks (10-doc corpus):**
- Indexing: 0.072ms per doc
- Retrieval precision @1: 20% | @3: 13.33%
- Context hit rate @3: 40%

**Tech Stack:** TypeScript, Node.js, React, Redis, Ollama (local LLM), SSE  
**Tests:** Chunking behavior, retrieval ranking, Redis memory, route contracts, SSE response shape

---

### **🧠 RAG System — Production-Ready Retrieval Pipeline** — *In Progress*
[**Repository**](https://github.com/pixelpitstop/RAG-project)  
Dockerized, production-oriented Retrieval-Augmented Generation pipeline with clean separation: retrieval system → API layer → evaluation harness.

**Built for:**
- Deployability, reproducibility, testability from day one
- FastAPI interface with full environment reproducibility
- End-to-end retrieval quality evaluation (often missing in RAG demos)
- pytest configuration, CI-ready test structure

**Tech Stack:** Python, FastAPI, Docker, docker-compose, LangChain-style retrieval, pytest  
**Key Files:** main.py, evaluate.py, Dockerfile, docker-compose.yml, quickstart.sh, verify_setup.sh

---

### **🌐 ShadowFox Learning Platform (v2)** — *Full-Stack*
[**Repository**](https://github.com/pixelpitstop/Shadowfox-website-v2)  
Full-stack learning platform monorepo for ShadowFox Technologies with polished Next.js 13 frontend and Node.js/Express backend.

**Integrations:**
- Google OAuth authentication
- Multiple Google Sheets integrations: auth logs, user certifications, internship apps, waitlist, campus ambassador programs
- JWT-based API authentication + CORS

**Tech Stack:**
- **Frontend:** Next.js 13+, React 18, TypeScript, Tailwind CSS, Framer Motion, NextAuth.js
- **Backend:** Node.js, Express, JWT, Google Sheets API
- **Database:** PostgreSQL/MongoDB

---

## 🛠️ Technical Skills

**Languages & Frameworks:** Python, JavaScript/TypeScript, C++, React, Node.js, Express, Next.js  
**AI/ML & Data:** XGBoost, scikit-learn, pandas, NumPy, SHAP, Matplotlib, Seaborn, Ollama, LangChain  
**Databases & Storage:** MongoDB, PostgreSQL  
**Tools & Platforms:** FastAPI, Streamlit, Docker, docker-compose, Google Earth Engine, Git, pytest, Redis  
**Domains:** Time-series forecasting, anomaly detection, recommendation systems, geospatial analysis, automotive diagnostics, micro-fraud detection, RAG systems

---

## 💡 Engineering Philosophy

I focus on **signal over noise** — models that generalize, metrics that matter, systems that survive real-world data.

I value **clean abstractions**, **explainability**, and **AI systems that work beyond notebooks** — combining rigorous ML with production-grade engineering.

---

## 🔍 What I'm Building Toward

Top-tier **AI/ML Engineering roles** with a long-term focus on scalable, high-impact intelligent systems across:
- Applied ML systems at production scale
- Time-series & behavioral analytics
- Automotive intelligence & autonomous systems
- Fraud detection & financial ML

---

📮 **Let's Connect**  
💬 Open to discussions on ML systems, full-stack AI projects, and opportunities in AI engineering.

**Email:** [jayasuryaa1785@outlook.com](mailto:jayasuryaa1785@outlook.com)  
**LinkedIn:** [linkedin.com/in/jayasuryaachandrasekar](https://linkedin.com/in/jayasuryaachandrasekar/)  
**Portfolio:** [jayasuryaa.vercel.app](https://jayasuryaa.vercel.app)
