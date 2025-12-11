# Predictive Maintenance for Railway Point Machines  
### Anomaly Detection using Machine Learning and Deep Learning

## Overview
This project focuses on identifying early-stage mechanical faults in **Indian Railways point machines** by analyzing real-world **current and voltage sensor data**.  
The goal is to support predictive maintenance workflows by flagging subtle anomalies in machine behaviour long before failures occur.  
:contentReference[oaicite:0]{index=0}

The system includes a complete data-processing pipeline, multiple anomaly-detection models, and utilities for validation, comparison, and long-term integration.

---

## Features

### 1. End-to-End Data Pipeline
- Handles raw sensor data ingestion, cleaning, normalization, and validation.  
- Includes monitoring and logging utilities to track model behaviour and ensure reproducibility.  
:contentReference[oaicite:1]{index=1}

### 2. Multiple Anomaly Detection Algorithms
The project evaluates several approaches to detect deviations across machines:

- **Isolation Forest**  
- **Local Outlier Factor (LOF)**  
- **LSTM Autoencoders** for capturing temporal patterns over continuous sensor readings  

These methods were compared to understand which performs best for early fault detection.  
:contentReference[oaicite:2]{index=2}

### 3. Real-World Sensor Dataset
- Works with thousands of actual current and voltage readings from operational railway point machines.  
- Focuses on detecting behavioural drift rather than only clear-cut failures.  
:contentReference[oaicite:3]{index=3}

### 4. Production-Oriented Structure
- Contains structured utilities for model evaluation and result comparison.  
- Designed to support long-term integration into a larger predictive maintenance workflow.  
:contentReference[oaicite:4]{index=4}

---

## Tech Stack
- **Python**  
- **Pandas**, **NumPy**  
- **scikit-learn** (Isolation Forest, LOF)  
- **TensorFlow / Keras** (LSTM Autoencoder)  
- **Custom logging utilities** for monitoring  
:contentReference[oaicite:5]{index=5}

---

## System Workflow

### 1. Data Collection  
Raw current and voltage sensor readings are gathered at regular intervals from railway point machines.

### 2. Preprocessing  
- Outlier removal (initial noise filtering)  
- Normalization  
- Time-series windowing for deep learning models  

### 3. Model Training & Evaluation  
Each anomaly detection technique is trained and evaluated on the processed dataset.  
LSTM autoencoders reconstruct normal behaviour and highlight deviations through reconstruction error.

### 4. Fault Flagging  
Outputs from different models are compared to ensure consistent detection of anomalies.  
This supports early warnings for railway maintenance teams.

---

## Project Goals
- Improve reliability of point machines using data-driven monitoring.  
- Reduce unplanned downtime by identifying patterns that precede mechanical faults.  
- Build a scalable and reproducible anomaly detection framework suitable for industrial environments.

---

## Status
This project was developed as part of academic work at SRM Institute of Science and Technology (2024–2025).  
It is structured to be extendable for future real-time predictive maintenance deployments.  
:contentReference[oaicite:6]{index=6}
