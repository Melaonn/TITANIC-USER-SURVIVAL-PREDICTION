# 🛳️ Titanic Survival Prediction - MLOps Project

This project aims to predict the survival of passengers on the Titanic using a robust MLOps pipeline. It integrates multiple tools and platforms across the lifecycle — from data ingestion to monitoring — offering a real-world production-grade ML system.

---

## 🚀 Overview

Using the popular Titanic dataset, this end-to-end system demonstrates:

- Data ingestion from GCP buckets  
- ETL orchestration with Apache Airflow  
- PostgreSQL integration  
- Feature engineering and storing using Redis  
- Model training and versioning  
- A Flask-based user-facing prediction app  
- Real-time drift detection and monitoring

---

## 🧰 Tech Stack & Workflow

### 📦 Data Storage & Ingestion
- **Google Cloud Storage (GCS)**: Titanic dataset is hosted in a GCP bucket.
- **Apache Airflow**: Used for scheduling and managing the ETL pipeline.
- **PostgreSQL**: Stores processed structured data from the CSV.
- **Psycopg2**: Python-PostgreSQL adapter used to insert and query data.

### 📓 Experimentation & Feature Engineering
- **Jupyter Notebooks**: For initial testing and exploratory data analysis.
- **Redis**: Serves as a lightweight feature store for serving and training.

### 🧠 Model Training & Versioning
- Feature extraction and preprocessing are integrated with the training process.
- Data and code versioning handled via Git and reproducible training scripts.

### 🌐 API Application
- **Flask App**: Simple web interface for user inputs and prediction output.
- Takes user details like age, gender, class, etc., and returns survival prediction.

### 📉 Drift Detection & Monitoring
- **Alibi Detect**: Monitors incoming data for drift in input distribution.
- **Prometheus & Grafana**: Real-time monitoring and visualization of model health metrics.
