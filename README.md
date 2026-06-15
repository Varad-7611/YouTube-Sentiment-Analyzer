# 🚀 AI-Powered YouTube Sentiment Insight Chrome Extension

## 📌 Project Overview

This project is an end-to-end **MLOps-based Machine Learning system** integrated with a **Chrome Extension** that provides real-time sentiment insights on YouTube content.

The system uses a trained NLP model to analyze text (comments/titles) and classify sentiment (positive/negative), delivering instant insights directly in the browser.

---

## 🎯 Features

* 🔍 Real-time sentiment analysis
* 🌐 Chrome Extension integration
* 🤖 Machine Learning model (TF-IDF + LightGBM)
* 📊 Experiment tracking using MLflow
* 🔁 Pipeline automation using DVC
* 🐳 Docker-based deployment
* ⚙️ CI/CD integration (GitHub Actions)

---

## 🧠 Tech Stack

* **Frontend:** Chrome Extension (HTML, CSS, JavaScript)
* **Backend:** Flask (Python)
* **Machine Learning:** Scikit-learn, LightGBM, TF-IDF
* **MLOps Tools:** DVC, MLflow
* **Deployment:** Docker
* **CI/CD:** GitHub Actions

---

## 🏗️ Project Structure

```
├── data/
│   ├── raw/
│   └── interim/
├── src/
├── flask_app/
├── mlartifacts/
├── dvc.yaml
├── params.yaml
├── Dockerfile
├── .github/workflows/
├── models/
└── README.md
```

---

## 🔄 Workflow

1. User interacts with Chrome Extension
2. Input is sent to Flask API
3. API processes text using trained model
4. Prediction is returned to extension
5. Sentiment insight is displayed

---

## ⚙️ DVC Pipeline

* Data Ingestion
* Data Preprocessing
* Model Training
* Model Evaluation

📸 **DVC Pipeline Screenshot:**
<img width="866" height="504" alt="image" src="https://github.com/user-attachments/assets/ac8ecc33-4153-40f6-a717-a243372cbfc0" />


---

## 📊 MLflow Tracking

MLflow is used for:

* Logging parameters
* Tracking metrics
* Storing model artifacts

📸 **MLflow UI Screenshot:**
<img width="1858" height="909" alt="Screenshot 2026-06-14 091432" src="https://github.com/user-attachments/assets/5fa5ad64-aa39-4cde-8a90-b3cef4edaf86" />


---

## 🖥️ Working Demo

📸 **Chrome Extension Output:**

<img width="816" height="426" alt="Screenshot 2026-06-14 101614" src="https://github.com/user-attachments/assets/a2312395-ac2c-485d-b3a6-c04b61d97fb1" />

<img width="1903" height="890" alt="Screenshot 2026-06-14 101402" src="https://github.com/user-attachments/assets/c267864f-248d-47f4-b117-9e3c7cd65d27" />

<img width="1879" height="897" alt="Screenshot 2026-06-14 101414" src="https://github.com/user-attachments/assets/8fd3aad3-c1b0-484a-a2c1-9796e8cd0f07" />

<img width="1828" height="825" alt="Screenshot 2026-06-14 101427" src="https://github.com/user-attachments/assets/e37109a6-57d1-4f15-b14c-81eb2c4581df" />



---

## 🐳 Docker Setup

```bash
docker build -t sentiment-app .
docker run -p 5000:5000 sentiment-app
```

---

## 🚀 How to Run Locally

```bash
git clone https://github.com/Varad-7611/YouTube-Sentiment-Analyzer.git
cd YouTube-Sentiment-Analyzer

pip install -r requirements.txt

dvc repro

python flask_app/app.py
```

---

## 📈 Future Improvements

* Deploy on AWS (EC2/S3)
* Add real-time monitoring (Evidently AI)
* Implement model retraining pipeline
* Improve UI/UX of extension

---

## ⭐ Conclusion

This project demonstrates a complete **MLOps pipeline integrated with a real-world application**, enabling scalable and reproducible machine learning deployment.
