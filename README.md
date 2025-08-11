# 🛒 LLMOps & AIOps Project 2: Flipkart Product Recommender System

![LLMOps](https://img.shields.io/badge/LLMOps-AIOps-blueviolet)
![Python](https://img.shields.io/badge/Python-3.12%2B-brightgreen)
![Docker](https://img.shields.io/badge/Docker-Ready-blue)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Deploy-blue)
![License](https://img.shields.io/badge/License-GPL--3.0-orange)

A modern, production-ready Flipkart Product Recommender System utilizing LLMOps and AIOps best practices. This solution leverages Large Language Models, RAG (Retrieval Augmented Generation), and scalable vector search to deliver smart, explainable, and contextual product recommendations. Features a modular and robust codebase, Dockerization, Kubernetes manifests, and observability via Prometheus and Grafana.

> 📁 **Repository:** `LLMOPS-AIOPS-Project2-FLIPKART-PRODUCT-RECOMMENDER-SYSTEM`

---

## 🚀 Project Highlights

- ⚡ **RAG-powered Recommendations:** Products are recommended using a Retrieval Augmented Generation chain and LLMs for context enrichment.
- 🔍 **Semantic & Vector Search:** Fast, scalable product similarity search.
- 📊 **Observability:** Out-of-the-box monitoring with Prometheus and Grafana manifests.
- 🏗️ **Modular Pipeline:** Easily extensible and maintainable; clean code separation.
- 🐳 **Dockerized:** Build, test, and run anywhere.
- ☸️ **Kubernetes-Ready:** Includes deployment manifests for scalable, cloud-native serving.
- 🎨 **Web App:** Interactive UI for users to get product recommendations.

---

## 🧠 Technical Stack

- **Python 3.12+**
- **Flask** (web app API)
- **RAG (Retrieval Augmented Generation)**
- **Vector Search** (custom or third-party)
- **Prometheus & Grafana** (monitoring & visualization)
- **Docker, Kubernetes**
- **Modern Python OOP & Pipeline Patterns**

---

## 🏗️ Project Structure

```bash
LLMOPS-AIOPS-Project2-FLIPKART-PRODUCT-RECOMMENDER-SYSTEM/
├── app.py                      # Flask app entry point
├── data/
│   └── flipkart_product_review.csv
├── flipkart/
│   ├── __init__.py
│   ├── config.py
│   ├── data_converter.py
│   ├── data_ingestion.py
│   └── rag_chain.py
├── grafana/
│   └── grafana-deployment.yaml
├── prometheus/
│   ├── prometheus-configmap.yaml
│   └── prometheus-deployment.yaml
├── static/
│   └── style.css
├── templates/
│   └── index.html
├── utils/
│   ├── __init__.py
│   ├── custom_exception.py
│   └── logger.py
├── Dockerfile
├── flask-deployment.yaml       # Kubernetes deployment for Flask app
├── FULL DOCUMENTATION.md
├── LICENSE
├── README.md
├── requirements.txt
├── setup.py
```

---

## ⚡ Installation & Usage

### 1. Clone the repository
```bash
git clone https://github.com/mdzaheerjk/LLMOPS-AIOPS-Project2-FLIPKART-PRODUCT-RECOMMENDER-SYSTEM.git
cd LLMOPS-AIOPS-Project2-FLIPKART-PRODUCT-RECOMMENDER-SYSTEM
```

### 2. Set up a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the application
```bash
python app.py
```
Or build and run with Docker:
```bash
docker build -t flipkart-recommender .
docker run -p 8000:8000 flipkart-recommender
```

### 5. Kubernetes Deployment
Apply the manifests to your cluster:
```bash
kubectl apply -f flask-deployment.yaml
kubectl apply -f prometheus/prometheus-configmap.yaml
kubectl apply -f prometheus/prometheus-deployment.yaml
kubectl apply -f grafana/grafana-deployment.yaml
```

---

## 📊 Observability & Monitoring

- **Prometheus:**  
  Monitors metrics from the recommender service.
- **Grafana:**  
  Visualizes metrics via dashboards (see `grafana/grafana-deployment.yaml`).

---

## 🧪 Example Usage

- **Product Recommendations:**  
  Users receive personalized product suggestions based on reviews, preferences, and context using advanced LLM & RAG techniques.

- **Web Interface:**  
  Simple, interactive UI for demo and production.

---

## 📚 Documentation

See [FULL DOCUMENTATION.md](FULL DOCUMENTATION.md) for detailed architecture, code structure, and configuration instructions.

---

## ✍️ Author

**Mohammed Zaheeruddin**  
🎓 First-Year B.Tech Student | AI/ML & GenAI Enthusiast  
🏫 Shetty Institute of Technology, Gulbarga  
📧 info.zaheerjk@gmail.com

---

## 📜 License

This project is licensed under the **GPL-3.0 License** – see the LICENSE file for details.

---

#### Key Features:
1. RAG and LLM-powered product recommender with semantic search
2. Modular, extensible, and observable codebase
3. Docker and Kubernetes ready for scalable production
4. Designed for research, education, and real-world applications
