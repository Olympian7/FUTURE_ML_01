---

# Future ML Internship – Project Repository

This repository contains all deliverables completed during the **Future ML Internship Programme**, structured as three independent tasks. Each task focuses on a different dimension of data and AI technology—ranging from forecasting and classification models to conversational AI.

---

## 📁 Repository Structure

```
FUTURE_ML/
│── Task 1/    # Forecasting model
│── Task 2/    # Churn prediction + business insight
│── Task 3/    # Dialogflow customer support chatbot
│── README.md  # This file
```

---

## 🧩 Task 1 – Retail Time Series Forecasting

### Objective

Build a forecasting pipeline to predict future retail sales using historical transaction data.

### Key Steps

* Performed exploratory data analysis and cleaned the transactional dataset
* Used **SARIMA** for time-series modelling
* Split data into training/testing and evaluated forecast accuracy
* Generated forward predictions and exported results
* Delivered a structured forecast that business teams can use for inventory planning

### Tools

Python, Pandas, Matplotlib, Statsmodels (SARIMA)

### Outputs

* Clean, reproducible notebook (`T1.ipynb`)
* Forecast visualizations
* Forecasted dataset (`sarima_forecast.csv`)

---

## 🔍 Task 2 – Customer Churn Prediction with Business Recommendation

### Objective

Create a churn prediction model for telecom customers and translate insights into business actions.

### Key Steps

* Cleaned and encoded Telco customer data
* Trained a logistic regression classifier
* Achieved **ROC-AUC ~0.83** with tuned threshold for better recall
* Classified customers into churn-risk bands
* Generated business insights with visualizations

### Tools

Python, Scikit-Learn, Pandas, Matplotlib

### Outputs

* Machine learning notebook (`T2.ipynb`)
* Plots (churn by tenure, charges, contract type, ROC curve, confusion matrix)
* Business-focused report (Markdown/PDF)

---

## 🤖 Task 3 – Dialogflow Chatbot Deployment

### Objective

Design and deploy a smart assistant capable of responding to user queries instantly.

### Key Steps

* Created intents for **weather**, **food ordering**, and **movies**
* Trained the chatbot using example utterances
* Implemented fallback conversation logic
* Tested using **Messenger integration** due to Web Demo issues
* Validated chatbot flows with live messages

### Tools

Dialogflow ES, Google Cloud Console, Messenger Platform

### Outputs

* Configured Dialogflow agent
* Working chatbot deployed on Messenger
* Intent design screenshots

---

## 🚀 Core Learning Outcomes Across Tasks

* **Data handling and EDA** on real-world datasets
* **Model development & evaluation**

  * Time series forecasting
  * Classification with imbalance handling
* **Business interpretation of analytics**
* **Conversational AI development and deployment**
* **Version control with Git + GitHub**

---

## 🧭 Next Possible Enhancements

* Automate forecasting and retraining pipelines
* Expand churn model with new features and model comparison (XGBoost / Random Forest)
* Add live data APIs to the chatbot (e.g., real weather)
* Integrate chatbot with web apps using Streamlit or Telegram

---

## ✔ Summary

This repository demonstrates end-to-end competency across **data engineering, machine learning, and conversational AI** through three hands-on tasks. The structure ensures each module stands alone but contributes to a cohesive portfolio of practical ML applications.


