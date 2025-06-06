# 📊 InsightDash

**InsightDash** is a real-time analytics dashboard built with Angular for querying and visualizing live metrics from Elasticsearch clusters. Designed for high-throughput environments, it supports multi-index querying, dynamic filters, and heatmap visualizations for rapid situational awareness.

Deployed via **Docker containers** and managed with **AWS ECS** and **CI/CD pipelines**, InsightDash offers plug-and-play data modeling and flexible integration with AI analysis services.

## 📌 Features

- 📈 **Live Analytics Views**:
  - Visual dashboards with line graphs, bar charts, and heatmaps
  - Elastic query builder with multi-index support
  - Alert overlays and dynamic filter panels

- 🔌 **API & AI Integration**:
  - REST APIs for custom analytics ingestion
  - Hooks for ML services to overlay anomaly detection

- 🐳 **Containerized Deployment**:
  - Dockerized frontend with Nginx reverse proxy
  - CI/CD-enabled rollout via AWS CodePipeline & ECS

## 🧰 Tech Stack

- **Frontend**: Angular, ngx-charts
- **Data Source**: Elasticsearch, Kibana APIs
- **Deployment**: Docker, AWS ECS, CodePipeline
- **Backend (Optional)**: Node.js or Flask for custom endpoints

## 🚀 Getting Started

```bash
git clone https://github.com/your-username/insightdash.git
cd insightdash
docker build -t insightdash-ui .
docker run -p 8080:80 insightdash-ui
