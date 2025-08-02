# Hotel Reservation Cancellation Prediction

This project is a web-based machine learning application designed to predict whether a hotel reservation will be canceled or not based on user input. The model is trained on historical booking data and deployed using Flask with Jenkins, Docker, and Google Cloud Platform integrations.

## 🚀 Features

- Web interface for predicting hotel reservation cancellations
- Machine learning model trained on structured hotel reservation data
- Jenkins pipeline for CI/CD
- Dockerized application for scalable deployment
- Hosted on Google Cloud Run using GCR and GCP Buckets for model and data management

---

## 🛠 Tech Stack

- **Frontend:** HTML, CSS (via Flask templates)
- **Backend:** Python (Flask)
- **ML Model:** Scikit-learn (loaded using `joblib`)
- **CI/CD:** Jenkins
- **Containerization:** Docker
- **Deployment:** Google Cloud Run & GCR
- **Storage:** GCP Buckets

---

## 🧠 Model Overview

- Accuracy: **89%**
- Dataset: **20,000 data points**, augmented to **38,000**
- Input features include:
  - Lead time
  - Number of special requests
  - Average room price
  - Arrival month and date
  - Market segment type
  - Number of weekend/week nights
  - Type of meal plan
  - Room type reserved

---

## 📁 Project Structure

```
Hotel Reservation/
│
├── application.py             # Main Flask app
├── Dockerfile                 # Docker configuration
├── Jenkinsfile                # Jenkins CI/CD pipeline
├── requirements.txt           # Python dependencies
├── setup.py                   # Package configuration
│
├── templates/                 # HTML templates
│   ├── home.html
│   ├── predict.html
│   ├── about.html
│   └── info.html
│
├── config/
│   └── paths_config.py        # Path to model output
│
├── artifacts/                 # Trained model artifacts
└── ...
```

---

## 🌐 Application Routes

| Route      | Description                                   |
| ---------- | --------------------------------------------- |
| `/`        | Home page                                     |
| `/predict` | Form to enter reservation details and predict |
| `/about`   | Project description                           |
| `/info`    | Additional project info                       |

---

## 🧪 How to Run Locally

```bash
# 1. Clone the repository
git clone <repo-url>
cd "Hotel Reservation"

# 2. Set up virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run the app
python application.py
```

Then go to `http://localhost:8080` in your browser.


