# Jayasuryaa Chandrasekar

**AI & Full-Stack Engineer** — building systems that work beyond notebooks and demos.

Final Year, B.Tech CSE-IoT | SRMIST Ramapuram (CGPA: 8.65/10)
Research Intern, CACS — IIT Madras | Ex-Research Intern, MS Swaminathan Research Foundation

📧 jayasuryaa1785@outlook.com • [LinkedIn](https://linkedin.com/in/jayasuryaachandrasekar/) • [Portfolio](https://jayasuryaa.vercel.app)

---

## Projects

### CANInsight — Vehicle Diagnostics & Telemetry Intelligence
[Repository](https://github.com/pixelpitstop/Canbus-project)

Complete automotive CAN bus diagnostics pipeline — from raw bytes to operator-facing insights.

**Pipeline:** Raw CAN logs → Signal Extraction → Rule-Based Diagnostics → Insight Generation → Streamlit Dashboard

- Parses raw CAN-like logs (timestamp + ID + hex) into structured byte arrays
- Extracts engineering signals: RPM, throttle %, speed, engine temp, brake %
- Detects operational events (overheating, RPM spikes, harsh braking) with severity scoring
- Streamlit dashboard: telemetry charts, trip score, max readings, alerts table, insight report

**Stack:** Python · Streamlit · pandas · structured event system

---

### Electricity Anomaly Detection System — Production-Grade ML
[Repository](https://github.com/pixelpitstop/Time-Series-Forecasting)

Production-oriented ML system for detecting anomalous electricity demand in the PJME hourly grid dataset.

**Architecture:** Raw Data → Feature Engineering → 24h XGBoost Forecast → Residual Engine → Threshold → Anomaly Flags → API/CLI

- Configurable anomaly threshold via residual quantile (99th percentile default)
- Per-anomaly-type evaluation: spike, drop, flatline with detection delay tracking
- Drift handling: threshold recalibration + model retraining
- Outputs: detection_metrics.json, anomaly_type_metrics.csv, scored_test_window.csv

**Stack:** Python · XGBoost · pandas · FastAPI · Streamlit · pytest · uvicorn

---

### Urban Thermal Equity Index (UTEI) — Chennai
[Repository](https://github.com/pixelpitstop/Urban-Thermal-Equity-Index-using-Machine-Learning)

Research-grade geospatial ML project introducing a novel metric to quantify heat distribution inequality across city neighborhoods. Built during MSSRF internship; currently extended at IIT Madras CACS.

**Formula:** LST (MODIS) + Humidity (IoT/weather) − NDVI (Sentinel-2)

- Lasso regression trained on fused geospatial dataset
- Per-location UTEI scores across Chennai
- Interactive Leaflet/Folium thermal equity heatmap
- First index combining vegetation, land temperature, and humidity for measuring thermal equity

**Stack:** Python · pandas · scikit-learn · Folium · Google Earth Engine · MODIS/Sentinel-2

---

### AI MUN Assistant — Local-First RAG Chatbot
[Repository](https://github.com/pixelpitstop/AI-Chatbot-project)

Production-grade AI assistant for Model United Nations delegates — complete local-first RAG system with streaming, memory, and structured generation.

- Document ingestion → chunking & embedding → persistent vector index
- Redis-backed short-term memory + file-backed strategy memory
- Argument generation: opening statements, counter-arguments, cross-questions
- SSE streaming for low-latency UX

**Benchmarks (10-doc corpus):** Indexing 0.072ms/doc · Retrieval precision @1: 20% · Context hit rate @3: 40%

**Stack:** TypeScript · Node.js · React · Redis · Ollama · SSE

---

### ShadowFox Learning Platform
[Repository](https://github.com/pixelpitstop/Shadowfox-website-v2)

Full-stack learning platform with Next.js 13 frontend and Node.js/Express backend — built and deployed for a live client.

- Google OAuth authentication + JWT-based API auth
- Google Sheets integrations: auth logs, certifications, internship apps, waitlist, campus ambassador
- Production deployment with CORS, environment management, and multi-route backend

**Stack:** Next.js 13 · React 18 · TypeScript · Tailwind CSS · Node.js · Express · PostgreSQL/MongoDB · NextAuth.js

---

### BrewBase CRM
[Repository](https://github.com/pixelpitstop/brewbase-crm)

Full-stack AI-integrated CRM built and deployed for a real client use case — AI automation at three distinct workflow points.

- Segment builder, message composer, and campaign debrief engine — each AI-assisted
- Next.js frontend + Express/PostgreSQL backend + BullMQ/Redis job queue
- Deployed across Railway, Vercel, Supabase, and Upstash

**Stack:** Next.js · Express · PostgreSQL · Redis · BullMQ · Upstash · Vercel · Railway

---

## Skills

**Languages:** Python · JavaScript/TypeScript · C++
**AI/ML:** XGBoost · scikit-learn · pandas · NumPy · SHAP · Ollama · LangChain
**Full-Stack:** React · Next.js · Node.js · Express · FastAPI · Streamlit
**Databases:** PostgreSQL · MongoDB · Redis
**Tools:** Docker · Git · pytest · Google Earth Engine
**Domains:** Automotive telemetry · Time-series forecasting · Anomaly detection · Geospatial ML · RAG systems · Fraud detection
