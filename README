# 🧠 Simple ML System Design

A minimal end-to-end machine learning system to demonstrate how to take a model from training to deployment in a scalable and reproducible way.

---

## 📌 Project Structure

```bash
simple-ml-system/
├── data/                  # Raw and processed data
├── notebooks/             # EDA and experimentation
├── src/                   # Source code
│   ├── training/          # Model training pipeline
│   ├── serving/           # FastAPI model server
│   └── utils/             # Helper functions
├── models/                # Serialized model artifacts
├── Dockerfile             # For containerization
├── requirements.txt       # Python dependencies
├── airflow_dag.py         # (Optional) Orchestration pipeline
├── prometheus.yml         # (Optional) Monitoring config
└── README.md
```

---

## 🧪 Tech Stack

- **Language**: Python 3.9+
- **ML Framework**: Scikit-learn / PyTorch / XGBoost
- **Serving**: FastAPI
- **Containerization**: Docker
- **Orchestration**: Airflow (optional)
- **Monitoring**: Prometheus + Grafana (optional)
- **Cloud Ready**: Can be deployed to GCP/AWS using Cloud Run/ECS

---

## 🚀 Key Components

### 1. Data Ingestion
- Ingests raw CSV/JSON data
- Performs basic cleaning and transformations

### 2. Model Training
- Uses a standard pipeline with train/test split
- Trains a classification/regression model
- Saves model using `joblib` or `torch.save()`

### 3. Model Serving
- FastAPI endpoint: `POST /predict`
- Loads the latest trained model from disk
- Returns predictions as JSON

### 4. CI/CD (Optional)
- GitHub Actions workflow to lint, test, and build Docker image
- Pushes to DockerHub or Artifact Registry

---

## 🔁 Sample API Usage

```bash
curl -X POST "http://localhost:8000/predict" \
     -H "Content-Type: application/json" \
     -d '{"feature_1": 5.3, "feature_2": 2.1}'
```

Response:
```json
{"prediction": "positive"}
```

---

## 📦 Getting Started

```bash
# Clone repo
git clone https://github.com/yourusername/simple-ml-system.git
cd simple-ml-system

# Install dependencies
pip install -r requirements.txt

# Train model
python src/training/train_model.py

# Start FastAPI server
uvicorn src.serving.app:app --reload
```

---

## 📊 Future Enhancements

- Switch to a cloud storage backend (GCS/S3)
- Add MLflow for experiment tracking
- Add monitoring with Prometheus + Grafana
- Deploy to GCP/AWS with Terraform/IaC

---

## 🤝 Contributions

Open to pull requests and improvements. Fork the repo, create a feature branch, and submit a PR!

---

Let me know your stack preference (e.g., PyTorch vs. Scikit-learn, Airflow vs. Prefect) and I can generate the actual repo code or README with code snippets filled in.
