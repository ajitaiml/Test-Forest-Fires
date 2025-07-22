# 🔥 Forest Fire Weather Index (FWI) Predictor

A production-ready machine learning web application built with Flask, designed to predict the Forest Fire Weather Index (FWI) based on meteorological inputs. This project demonstrates a full ML lifecycle — from data preprocessing and model training to deployment using AWS Elastic Beanstalk.

---

## 📌 Overview

Forest fires pose a severe environmental threat. Predicting the FWI helps with early warning and proactive fire prevention measures. This app uses a Ridge Regression model to predict FWI from key environmental parameters.

---

## 🚀 Live Demo

🔗 [Try the Live App](http://testforestfires-env-1.eba-wapp9iuf.ap-south-1.elasticbeanstalk.com/)

---

## 🧠 Machine Learning Workflow

- 📊 Data collection & cleaning  
- ⚙️ Feature engineering & scaling  
- 🧮 Ridge Regression model training  
- 💾 Model serialization (`ridge.pkl`, `scaler.pkl`)  
- 🌐 Flask web integration  
- ☁️ Deployment using AWS Elastic Beanstalk  

---

## 📈 Features Used

| Feature     | Description                       |
|-------------|-----------------------------------|
| Temperature | Ambient temperature (°C)          |
| RH          | Relative humidity (%)             |
| Ws          | Wind speed (km/h)                 |
| Rain        | Rainfall (mm)                     |
| FFMC        | Fine Fuel Moisture Code           |
| DMC         | Duff Moisture Code                |
| ISI         | Initial Spread Index              |
| Classes     | Fire Occurrence (0 or 1)          |
| Region      | Region Index (0 or 1)             |

---

## 🛠 Tech Stack

| 🧩 Component      | 🛠 Technologies & Tools                                |
|-------------------|--------------------------------------------------------|
| 🖼️ Frontend       | ![HTML](https://img.shields.io/badge/-HTML-E34F26?logo=html5&logoColor=white) ![CSS](https://img.shields.io/badge/-CSS-1572B6?logo=css3&logoColor=white) |
| ⚙️ Backend        | ![Flask](https://img.shields.io/badge/-Flask-000000?logo=flask&logoColor=white) |
| 📊 ML Model       | ![Scikit-learn](https://img.shields.io/badge/-Scikit--Learn-F7931E?logo=scikit-learn&logoColor=white) (Ridge Regression) |
| ☁️ Deployment     | ![AWS](https://img.shields.io/badge/-AWS%20Elastic%20Beanstalk-232F3E?logo=amazonaws&logoColor=white) |
| 🗃️ Version Control| ![Git](https://img.shields.io/badge/-Git-F05032?logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/-GitHub-181717?logo=github&logoColor=white) |
| 🧪 Environment    | ![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white) |

---

## 🗂 Project Structure

| Path                        | Description                                                  |
|-----------------------------|--------------------------------------------------------------|
| `.ebextensions/`           | AWS Elastic Beanstalk environment configuration files        |
| └── `python.config`        | Script to install Python packages on the EC2 instance        |
| `model/`                   | Stores serialized ML components                              |
| ├── `ridge.pkl`            | Trained Ridge Regression model                               |
| └── `scaler.pkl`           | StandardScaler used for preprocessing                        |
| `templates/`               | HTML templates used by Flask (Jinja2)                        |
| └── `index.html`           | Main input/output web page                                   |
| `app.py`                   | Main Flask app handling routes and predictions               |
| `train_model.ipynb`        | Jupyter notebook for training and saving the ML model        |
| `requirements.txt`         | Python dependencies for running the app                      |
| `runtime.txt`              | Python runtime version specification for AWS deployment      |
| `README.md`                | Project overview and documentation                           |

---

## 📬 Contact

If you have any suggestions or feedback, feel free to connect!

📧 ajitsingh@example.com  
🔗 [LinkedIn](https://www.linkedin.com/in/your-profile/)  
