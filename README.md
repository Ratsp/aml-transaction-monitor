# AML Transaction Monitoring System

> Graph-based Anti-Money Laundering detection engine inspired by real-world AML failures in global banking systems (e.g., Barclays FCA fine).

---

## 🚨 Problem

Traditional AML systems:

* Generate **90–95% false positives**
* Fail to detect **coordinated laundering networks**

This project solves that using:
👉 **Graph analytics + Machine Learning**

---

## 🧠 Solution Overview

* Detects **money mule networks**
* Uses **transaction graph relationships**
* Combines **unsupervised ML + anomaly detection**

---

## 🏗️ Architecture

Transaction Stream
→ Kafka
→ Feature Engineering
→ Neo4j Graph DB
→ Community Detection (Louvain)
→ Autoencoder (PyTorch)
→ Risk Scoring API (FastAPI)
→ Dashboard (React + Sigma.js)

---

## 🧰 Tech Stack

| Layer      | Technology             |
| ---------- | ---------------------- |
| Streaming  | Apache Kafka           |
| Graph DB   | Neo4j                  |
| ML Model   | PyTorch, scikit-learn  |
| Backend    | FastAPI                |
| Frontend   | React + Sigma.js       |
| Deployment | Docker, GitHub Actions |

---

## 📊 Dataset

* **PaySim Dataset**
* 6M synthetic transactions
* Mimics real mobile money fraud patterns

---

## ⚡ Quick Start

### 1. Clone Repo

```bash
git clone https://github.com/YOUR_USERNAME/aml-transaction-monitor.git
cd aml-transaction-monitor
```

### 2. Setup Environment (Windows)

```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Run Services

```bash
docker-compose up -d
```

---

## 📈 Expected Outcomes

* Detect hidden fraud rings
* Reduce false positives
* Improve AML compliance efficiency

---

## 🚀 Project Roadmap

* [ ] Data Pipeline (Kafka + Processing)
* [ ] Graph Construction (Neo4j)
* [ ] ML Model (Fraud Detection)
* [ ] API Development
* [ ] Dashboard Visualization
* [ ] Deployment

---

## 💼 Why This Project Matters

Financial institutions lose billions due to weak AML systems.

This project demonstrates:

* Real-world fintech problem solving
* Scalable system design
* Data engineering + ML integration

---

## 👤 Author

**Ratnali Pawar**
B.Tech AI & Data Science

---