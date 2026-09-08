# Auxia: Next-Gen Autonomous Supply Chain & Intelligent Logistics Platform

## Problem Statement & Vision
Modern supply chains face significant friction from reactive management. **Auxia** offers a unified **Logistics Command Center** that converts static supply chains into self-healing, predictive fulfillment networks.

## Key Innovation & Value Proposition
- **System Architecture:** Combines Reinforcement Learning (RL) for grid-based warehouse picking with graph-based dynamic routing across distributed transit nodes.
- **Differentiator:** End-to-end adaptive routing engine powered by Machine Learning. Auxia proactively forecasts weather and traffic bottlenecks, executing real-time automated rerouting before disruptions occur.

---

## Key Capabilities

- **Command & Control Dashboard**: Real-time operational overview tracking fleet telemetry, inventory levels, and order pipelines.
- **Autonomous Grid Fulfillment**: PPO-trained RL agents navigating complex warehouse environments to execute automated picking.
- **3D Workspace Twin**: Interactive digital twin rendering warehouse operations via Three.js.
- **Predictive Risk Assessment**: Multi-variable disruption scoring engine combining live weather streams and traffic analytics.
- **Adaptive Rerouting Matrix**: Graph-based path recalculation algorithm triggered by real-time risk alerts.
- **GenAI Disruption Insights**: Natural language risk context and recommended mitigation steps powered by Google Gemini.

---

## Algorithmic Foundation

Auxia incorporates specialized AI models and optimization algorithms:
- **XGBoost Classifier**: Multi-factor warehouse selection based on inventory proximity, workload distribution, and fulfillment capacity.
- **Dijkstra's Shortest Path**: Graph algorithm computing optimal transit corridors across the 22-node distribution network.
- **Proximal Policy Optimization (PPO)**: Deep RL framework for micro-navigation and collision avoidance on warehouse floors.
- **LightGBM Predictor**: Gradient boosted decision trees trained to forecast transit delays and route safety indices.

---

## Tech Stack & Architecture

### System Technologies
- **Frontend Layer**: React.js, Three.js, React Three Fiber, Tailwind CSS.
- **Backend Services**: FastAPI async gateway with WebSocket feeds for real-time telemetry streaming.
- **Data & Cloud Infrastructure**: Firebase Realtime Database for state synchronization, GCP for cloud hosting.

---

## Getting Started

### Prerequisites
- Python 3.10+
- Node.js 20+
- Service account key (`serviceAccountKey.json`) in `auxia_p1/`
- Environment config (`backend/.env`) with `GOOGLE_MAPS_API_KEY` and `GEMINI_API_KEY`

### 1. Start Backend Services
```bash
cd backend
pip install -r requirements.txt
python run_backend.py
```

### 2. Launch Control Panel
```bash
cd frontend
npm install
npm run dev
```

Open `http://localhost:5173` in your browser.

---
### Resources
- **Project Demo:** [Watch Video Demonstration]([https://drive.google.com/file/d/1_e_FabP5ld-Hk2iZ5TubcSKPOj4peNUV/view](https://docs.google.com/videos/d/1ctacpIknfGteZgplpzDnB8O1b9h0ZrJtUvL-n3WEpCI/play?usp=sharing))
