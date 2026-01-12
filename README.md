# 🚀 Optimus Data Pipeline

> **Hybrid Data Engineering System** for Financial Analysis.
> *Automated ingestion, containerized storage, and object-oriented analysis.*

![Status](https://img.shields.io/badge/Status-Active_Development-green)
![Docker](https://img.shields.io/badge/Docker-Containerized-blue?logo=docker)
![Java](https://img.shields.io/badge/Java-Analysis_Core-orange?logo=openjdk)
![Python](https://img.shields.io/badge/Python-Ingestion-yellow?logo=python)

## 📖 Overview
**Optimus** is a proof-of-concept pipeline designed to simulate a real-world DataOps environment. It orchestrates the lifecycle of financial data (Bitcoin metrics) through distinct, decoupled layers:

1.  **Ingestion Layer (Python):** Fetches real-time market data from external APIs.
2.  **Storage Layer (Docker & MySQL):** Persists data in an isolated, containerized relational database.
3.  **Analysis Layer (Java OOP):** Applies business logic to detect market trends (Bullish/Bearish).
4.  **Orchestration (Bash):** Automates the entire workflow in a Linux environment.

## 🏗 Architecture

| Component | Tech Stack | Responsibility |
| :--- | :--- | :--- |
| **Ingestion** | Python 3, Requests | Connects to CoinGecko API and parses JSON data. |
| **Storage** | Docker, MySQL 8.0 | Isolated persistence layer with persistent volumes. |
| **Logic** | Java 17 (OOP) | Data processing, average calculation, and trend detection. |
| **Control** | Bash Scripting | Crontab/Script based automation of the pipeline. |

## 🛠 Prerequisites
* **OS:** Ubuntu Server / Linux (Recommended)
* **Containerization:** Docker & Docker Compose
* **Languages:** Python 3.10+, Java 17 (JDK)

## 📂 Project Structure
```text
Optimus-Data-Pipeline/
├── docker/         # Infrastructure as Code (Docker Compose)
├── ingestion/      # Python scripts for API Data Fetching
├── analysis/       # Java Source Code for Business Logic
└── scripts/        # Bash orchestration scripts
