# AIML-MidTerm-AI-Crime-Pattern-Prediction

# 🛡️ AI-Powered Crime Pattern Predictor & Prevention Assistant

An intelligent, modular, and scalable crime analytics platform built to revolutionize public safety by leveraging AI/ML, data visualization, and natural language interfaces. This system predicts crime trends, identifies high-risk zones, automates reporting, and enables smart decision-making for law enforcement agencies.

---

## 🔍 Project Overview

This project aims to:

- 📈 Predict crime trends using spatiotemporal data and ML.
- 🗺️ Visualize high-risk zones and clusters across India.
- 📊 Deliver actionable insights via interactive dashboards.
- 🤖 Automate intelligence reports using LLMs (Large Language Models).
- 🛰️ Enable integration with digital policing platforms (IoT, CCTV, drones).
- 🌐 Offer multilingual, mobile-first interfaces for better accessibility.

---

## 🎯 Objectives

- Analyze multi-dimensional crime datasets (2020–2024).
- Forecast future crime loads by region and type.
- Identify statistically significant crime clusters.
- Provide real-time, dynamic dashboards for officers and policymakers.
- Automate natural language reports and Q&A using LLMs.
- Architect for integration with live feeds (CCTV, drones, 112).
- Recommend intelligent, predictive patrolling routes.
- Ensure mobile responsiveness and multilingual access.
- Support replicability across all Indian states.

---

## 📦 Dataset

**Source**: [CRIMES-IN-INDIA-2020-TO-2024](https://github.com/datameet/crime-in-india)  
**Records**: 1.2M+ anonymized entries  
**Attributes Include**:
- Year, Month of Occurrence
- Latitude, Longitude
- Crime Category/Subcategory
- Victim/Offender Demographics
- Legal Status (Chargesheeted, Pending, Convicted)
- Administrative Hierarchy (State → District → Police Station)

**Preprocessing Techniques**:
- Cleansing, normalization, imputation, encoding
- Feature engineering (recurrence rate, festival flags)
- Spatial clustering (DBSCAN/KMeans)
- Validation using NCRB official records

---

## 🧠 Methodology

### 1. Data Integration  
- GitHub, government portals, and APIs merged and harmonized.

### 2. EDA & Visualization  
- Heatmaps, seasonal analysis, gender-vulnerability matrices.

### 3. ML Modeling  
- Classification: Random Forest, XGBoost  
- Forecasting: ARIMA, SARIMA, Prophet  
- Clustering: DBSCAN, KMeans  
- Evaluation: AUC-ROC, Confusion Matrix, RMSE

### 4. Geo-Mapping  
- Plotly + Leaflet + Folium for live map overlays.

### 5. LLM Integration  
- Open-source models from HuggingFace  
- Natural language Q&A and auto-reporting

---

## 🖼️ Results

- 📈 **Cybercrime increased 180% (2020–2024)**
- 🧮 **87%+ model accuracy** for short-term forecasts
- 🗺️ **Real-time crime maps** by region, category, and time
- 📋 **District safety scores** and automated strategic insights
- 📆 **Predictive patrolling scheduler** based on time-of-day & density

---

## 🧱 System Architecture

graph TD
  UI[Frontend (React + Tailwind)]
  API[Flask REST API]
  ML[ML Models (.pkl)]
  DB[(PostgreSQL DB)]
  Cloud[AWS EC2/S3/Lambda]
  
  UI --> API
  API --> ML
  API --> DB
  ML --> DB
  DB --> UI
  API --> Cloud
