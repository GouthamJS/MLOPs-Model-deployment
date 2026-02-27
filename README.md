# Production-Ready MLOps Pipeline Project

This repository demonstrates the implementation of a production-style Machine Learning system designed with **reproducibility, automation, and deployment reliability** in mind.

Instead of focusing only on model training, this project emphasizes building a complete, deployable ML workflow aligned with modern MLOps practices.

---

## 🚀 What This Project Demonstrates

✔ End-to-end ML pipeline implementation  
✔ Experiment tracking and model versioning  
✔ Containerized deployment  
✔ CI/CD automation  
✔ Production-grade API serving  

The objective is to simulate how ML systems operate in real-world engineering environments.

---

## 🏗 System Design

The workflow follows a structured pipeline:

1. Data ingestion and preprocessing  
2. Model training and evaluation  
3. Experiment tracking using **MLflow**  
4. Model artifact management  
5. API wrapping using **FastAPI / Flask**  
6. Production serving via **Gunicorn**  
7. Containerization using **Docker**  
8. CI/CD automation using **GitHub Actions**  
9. Image publishing to **Docker Hub**  

---

## 🛠 Core Technologies

- **Python**
- **Scikit-learn**
- **MLflow**
- **DagsHub**
- **FastAPI / Flask**
- **Gunicorn**
- **Docker**
- **Docker Hub**
- **GitHub Actions**

---

## 📁 Repository Layout

```
.
├── src/                  # Training logic and pipeline scripts
├── app/                  # REST API implementation
├── models/               # Stored model artifacts
├── data/                 # Dataset files
├── notebooks/            # Experimentation & EDA
├── .github/workflows/    # CI/CD configurations
├── Dockerfile            # Container build instructions
├── requirements.txt      # Dependency definitions
└── README.md
```

---

## ⚙️ Local Development Setup

### Clone Repository

```bash
git clone https://github.com/YOUR-USERNAME/ML-OPs-Model-deployment.git
cd ML-OPs-Model-deployment
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Train Model

```bash
python src/train.py
```

Experiments and metrics are logged using **MLflow**.

---

## 🌐 Running the API

```bash
uvicorn app.main:app --reload
```

Access locally at:

```
http://127.0.0.1:8000
```

---

## 🐳 Containerized Execution

### Build Image

```bash
docker build -t mlops-pipeline .
```

### Run Container

```bash
docker run -p 8000:8000 mlops-pipeline
```

This ensures consistent runtime behavior across environments.

---

## 🔁 Continuous Integration

The CI workflow includes:

- Automated pipeline validation on push
- Dependency installation checks
- Docker image build process
- Deployment-ready artifact generation

---

## 📌 Engineering Highlights

- Designed for reproducibility across systems
- Environment isolation using Docker
- Structured experiment tracking
- Modular training and serving architecture
- Automation-driven workflow

---

## 🎯 Key Takeaways

This project reflects practical exposure to:

- Building ML systems beyond notebooks
- Managing experiments in a structured way
- Bridging ML development with DevOps practices
- Deploying containerized ML applications
- Implementing CI/CD for ML workflows

---

## 📜 License

MIT License
