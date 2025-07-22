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


| Category              | Tool                                                                 | Usage                                                                 |
|-----------------------|----------------------------------------------------------------------|-----------------------------------------------------------------------|
| Programming Language  | ![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white) | Base language for model building, preprocessing, and app logic       |
| Modeling              | ![TensorFlow](https://img.shields.io/badge/-TensorFlow-FF6F00?logo=tensorflow&logoColor=white) | Deep learning library used to build the ANN model                    |
| Modeling              | ![Keras](https://img.shields.io/badge/-Keras-D00000?logo=keras&logoColor=white) | High-level API to define and train the ANN model on top of TensorFlow |
| Web App               | ![Streamlit](https://img.shields.io/badge/-Streamlit-FF4B4B?logo=streamlit&logoColor=white) | Framework to build and deploy an interactive web app for predictions |
| Preprocessing         | ![Scikit-learn](https://img.shields.io/badge/-Scikit--learn-F7931E?logo=scikit-learn&logoColor=white) | Used for scaling, encoding, and preprocessing tabular data          |


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

]
