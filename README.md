# AML Transaction Monitoring System

> Graph-based Anti-Money Laundering detection engine built to address
> the AML control failures seen across major UK banks in 2024–2025
> (Barclays £43M FCA fine, 2025).

## Problem
Rule-based AML systems generate 95% false-positive alerts and miss
network-level laundering schemes. This system uses graph analytics
to detect money mule rings invisible to single-transaction analysis.

## Architecture
Transaction Feed → Kafka → Feature Engineering
→ Neo4j Graph → Louvain Community Detection
→ PyTorch Autoencoder → Risk Scoring API
→ React Dashboard with Sigma.js Graph Visualization

## Tech Stack (100% Free)
| Layer      | Technology                   |
|------------|------------------------------|
| Streaming  | Apache Kafka (Docker)        |
| Graph DB   | Neo4j Community Edition      |
| ML Model   | PyTorch + scikit-learn       |
| Backend    | FastAPI (Python)             |
| Frontend   | React + Sigma.js             |
| CI/CD      | GitHub Actions               |
| Hosting    | Render.com + Vercel (free)   |

## Dataset
PaySim: 6M synthetic mobile money transactions
Source: kaggle.com/datasets/ealaxi/paysim1

## Quick Start
```bash
git clone git@github.com:YOUR_USERNAME/aml-transaction-monitor.git
cd aml-transaction-monitor
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
docker-compose up -d
```

## Project Status
- [ ] Phase 1: Data pipeline (Weeks 1–2)
- [ ] Phase 2: ML model (Weeks 3–4)
- [ ] Phase 3: Dashboard (Weeks 5–6)
- [ ] Phase 4: Deployment (Weeks 7–10)

## Why I Built This
Barclays was fined £43M by the FCA in 2025 for AML control failures.
This project builds the continuous transaction monitoring system that
financial crime compliance teams need to prevent exactly these failures.
