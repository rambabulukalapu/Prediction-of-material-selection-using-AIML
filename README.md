
# 🔍 Prediction of Material Selection Using AI-ML

This repository contains a machine learning-based intelligent system for selecting optimal engineering materials. The model uses the Random Forest algorithm to predict and rank materials based on mechanical and thermal properties such as tensile strength, hardness, density, and thermal conductivity. It automates the traditionally manual process, enabling efficient, accurate, and cost-effective material selection.

---

## 📌 Abstract

Material selection is vital for performance, cost, and sustainability in manufacturing. Traditional methods are time-consuming and subjective. This project uses Random Forest—a robust machine learning algorithm—to automate material selection using data-driven insights. The model achieved an accuracy of 94%, significantly improving decision-making time and reliability. The system is deployed with a Flask API for real-time use.

---

## 🧠 Technologies Used

- Python  
- Pandas, NumPy – Data preprocessing  
- Scikit-learn – ML modeling (Random Forest, Logistic Regression, SVM)  
- Matplotlib, Seaborn – Visualization  
- Flask – REST API backend  
- Render – Deployment  
- Joblib – Model serialization  
- Postman – API testing  

---

## 📁 Dataset

The dataset consists of 10,000+ rows with the following key features:

- Tensile Strength (MPa)  
- Hardness (BHN)  
- Density (g/cm³)  
- Thermal Conductivity (W/mK)  
- Elastic Modulus (GPa)  
- Cost per Unit (₹/kg)  
- Target (Material Category)  

📂 File used: `Data.csv`

---

## 🛠️ How It Works

### 1. Data Preprocessing
- Handling missing values with mean imputation
- Outlier removal using Z-score
- Scaling with StandardScaler
- Categorical encoding using LabelEncoder

### 2. Model Training
- Random Forest Classifier (best performing)
- GridSearchCV for hyperparameter tuning
- Evaluation metrics: Accuracy, Precision, Recall, F1-score

### 3. Deployment
- Model served via Flask API
- Hosted using Render
- Input material properties → Output best-fit material category

---

## 🔗 API Usage

### Endpoint
```bash
POST /predict
```

### Sample Request
```json
{
  "feature1": 500,
  "feature2": 1200,
  "feature3": 200000,
  "feature4": 0.75
}
```

### Sample Response
```json
{
  "Prediction": 1
}
```

---

## 📈 Model Performance

| Metric      | Value     |
|-------------|-----------|
| Accuracy    | 94%       |
| Precision   | 93%       |
| Recall      | 91%       |
| F1-Score    | 92%       |
| Prediction Time | < 2 sec |

---

## 🧪 Applications

- 🏭 **Manufacturing** – Optimal raw material choice  
- 🚗 **Automotive** – Lightweight and impact-resistant materials  
- 🏗️ **Construction** – Durable and corrosion-resistant materials  
- 🧬 **Biomedical** – Biocompatible materials for implants  
- 🔋 **Energy** – Efficient thermal/electrical materials  
- ⚙️ **Defense** – Strong, lightweight armor materials  

---

## 👨‍💻 Project Contributors

- **Lukalapu Rambabu** – ML Modeling, Deployment  
- **D. Appalanaidu** – Data Preprocessing  
- **A. Thirumala Raju** – EDA & Feature Engineering  
- **K. Karthik** – API Development & Testing  

🧑‍🏫 Guided by: Mr. T. Ashok Kumar, M.Tech  
🏛️ Department of Mechanical Engineering  
📍 Narasaraopeta Engineering College, Andhra Pradesh  
🗓️ Project Submitted: April 2025

---

## 📬 Contact

- 📧 Email: [rambabulukalapu143@gmail.com](mailto:rambabulukalapu143@gmail.com)  
- 🔗 LinkedIn: https://www.linkedin.com/in/lukalapu-rambabu-526854240/  

---

> 📝 *This is a final-year B.Tech project submitted to JNTUK, showcasing the integration of AI/ML in material science for real-world industrial applications.*
