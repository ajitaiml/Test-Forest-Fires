# 🔥 Forest Fire Weather Index (FWI) Prediction

A production-ready machine learning web application built with **Flask**, designed to predict the **Forest Fire Weather Index (FWI)** based on meteorological inputs. This project demonstrates a full ML lifecycle — from data preprocessing and model training to deployment using **AWS Elastic Beanstalk**.

---

## 📌 Overview

Forest fires pose a severe environmental threat. Predicting the **FWI** helps in early warning and proactive measures. This application accepts key environmental features and predicts the FWI using a **Ridge Regression model** trained on historical data.

---

## 🚀 Live Demo

> 🔗 [Deployed App (AWS Elastic Beanstalk)](https://your-deployment-url.com)  
> *(Replace with your actual URL if available)*

---

## 🧠 Machine Learning Workflow

- **Data Collection** and Cleaning
- **Feature Engineering** and Scaling
- **Model Training** using Ridge Regression
- **Model Serialization** (`ridge.pkl`, `scaler.pkl`)
- **Web Interface Integration** using Flask
- **Deployment** to AWS using `.ebextensions` config

---

## 📈 Features Used

| Feature        | Description                        |
|----------------|------------------------------------|
| Temperature    | Ambient temperature (°C)           |
| RH             | Relative humidity (%)              |
| Ws             | Wind speed (km/h)                  |
| Rain           | Rainfall (mm)                      |
| FFMC           | Fine Fuel Moisture Code            |
| DMC            | Duff Moisture Code                 |
| ISI            | Initial Spread Index               |
| Classes        | Fire Occurrence (0 or 1)           |
| Region         | Region Index (0 or 1)              |

---

## 🛠️ Tech Stack

| Layer        | Tools                                |
|--------------|--------------------------------------|
| Frontend     | HTML, CSS (custom styled template)   |
| Backend      | Flask (Python)                       |
| ML Model     | Scikit-learn (Ridge Regression)      |
| Deployment   | AWS Elastic Beanstalk (`.ebextensions`) |
| Versioning   | Git & GitHub                         |

---

## 🗂 Project Structure

