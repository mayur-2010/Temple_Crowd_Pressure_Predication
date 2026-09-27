# Temple and Religious Gathering Crowd Stampede Pressure Index Prediction

## 📌 Project Overview

**Temple and Religious Gathering Crowd Stampede Pressure Index Prediction** is a Machine Learning project designed to predict crowd pressure levels during temple events, religious gatherings, festivals, and other crowded situations.

The system analyzes factors such as crowd density, crowd inflow, crowd outflow, weather conditions, corridor width, event conditions, and other crowd-related parameters.

The project provides two main outputs:

1. **Crowd Pressure Index** – A numerical value predicted using Regression.
2. **Risk Alert Level** – A classification such as:

   * Safe
   * Moderate
   * Critical

The main purpose of the system is to support early identification of potentially dangerous crowd conditions.

---

## 🎯 Objectives

* Predict the **Crowd Pressure Index** using Machine Learning.
* Identify different levels of crowd risk.
* Analyze important factors affecting crowd pressure.
* Provide an early warning mechanism for high-pressure situations.
* Help authorities understand crowd conditions and take preventive measures.
* Build a data-driven system for crowd safety management.

---

## 🚨 Importance of the Project

Large religious gatherings can create high crowd density, especially in narrow corridors, entrances, exits, and waiting areas.

If crowd pressure increases beyond a safe level, it may create dangerous conditions.

This project uses historical and simulated crowd-related data to predict crowd pressure and identify the corresponding risk level.

The predicted information can potentially support decisions such as:

* Crowd diversion
* Entry control
* Exit management
* Route management
* Additional security deployment
* Emergency preparedness

---

## 🧠 Machine Learning Approach

The project uses two Machine Learning approaches.

### 1. Regression

Regression is used to predict the numerical:

**Crowd Pressure Index**

Example:

```text
Crowd Pressure Index = 72.45
```

### 2. Classification

Classification is used to determine the risk level:

```text
Safe
Moderate
Critical
```

---

## 📊 Dataset

The project uses a crowd-flow dataset containing information related to crowd movement, environmental conditions, event conditions, and crowd density.

Example features include:

* Crowd Density
* Inflow Rate
* Outflow Rate
* Corridor Width
* Temperature
* Humidity
* Rainfall
* Event Type
* Event Day
* Average Speed
* Waiting Time
* Crowd Pressure Index
* Risk Alert Level

Dataset file used in this project:

```text
Temple_Crowd_Pressure_Dataset_20000.xlsx
```

---

## 🔧 Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* OpenPyXL
* Joblib

### Development Environment

* Jupyter Notebook
* Google Colab
* VS Code

---

## 🤖 Machine Learning Algorithms

The project can use the following algorithms:

### Regression Models

* Linear Regression
* Random Forest Regressor

### Classification Models

* Logistic Regression
* Random Forest Classifier

Random Forest can be used because it can handle multiple numerical and categorical features and can model non-linear relationships.

---

## 🔄 Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Cleaning
   ↓
Missing Value Handling
   ↓
Exploratory Data Analysis
   ↓
Feature Selection
   ↓
Data Preprocessing
   ↓
Train-Test Split
   ↓
Machine Learning Model
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Crowd Pressure Prediction
   ↓
Risk Level Classification
```

---

## 🧹 Data Preprocessing

The following preprocessing steps are performed:

1. Load the Excel dataset.
2. Check dataset shape.
3. Check column names.
4. Check missing values.
5. Remove or handle missing values.
6. Convert categorical variables into numerical form.
7. Select input and target variables.
8. Split the dataset into training and testing sets.

Example:

```python
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)
```

---

## 📈 Model Evaluation

### Regression Metrics

The regression model can be evaluated using:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

Example:

```text
MAE
MSE
RMSE
R² Score
```

### Classification Metrics

The classification model can be evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* Classification Report

---

## 📌 Expected Output

The system produces a numerical Crowd Pressure Index.

Example:

```text
Predicted Crowd Pressure Index: 78.35
Risk Alert Level: Critical
```

Another example:

```text
Predicted Crowd Pressure Index: 42.18
Risk Alert Level: Moderate
```

---

## 🚦 Risk Levels

The project uses three risk categories.

| Risk Level | Description                                       |
| ---------- | ------------------------------------------------- |
| Safe       | Crowd pressure is within a relatively low range   |
| Moderate   | Crowd pressure requires monitoring                |
| Critical   | High crowd pressure requiring immediate attention |

The exact thresholds should be defined from the project's dataset and validation methodology rather than assumed to represent real-world emergency standards.

---

## 📊 Data Analysis

Exploratory Data Analysis is performed to understand relationships between different variables.

Important analysis includes:

* Crowd density analysis
* Inflow and outflow analysis
* Weather analysis
* Event-day analysis
* Crowd pressure distribution
* Correlation analysis
* Risk-level distribution

Example visualizations:

* Histogram
* Bar Chart
* Scatter Plot
* Correlation Heatmap
* Box Plot

---

## 📁 Project Structure

```text
Temple-Crowd-Pressure-Prediction/
│
├── Temple_Crowd_Pressure_Dataset_20000.xlsx
│
├── Crowd_Pressure_Prediction.ipynb
│
├── README.md
│
├── requirements.txt
│
├── models/
│   ├── regression_model.pkl
│   └── classification_model.pkl
│
├── graphs/
│   ├── correlation_heatmap.png
│   ├── crowd_density.png
│   └── risk_distribution.png
│
└── screenshots/
    ├── dataset.png
    ├── model_output.png
    └── dashboard.png
```

---

## 💻 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Temple-Crowd-Pressure-Prediction.git
```

Go to the project folder:

```bash
cd Temple-Crowd-Pressure-Prediction
```

Install required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl joblib
```

---

## ▶️ How to Run

### Step 1

Open the project in:

```text
Jupyter Notebook
```

or

```text
Google Colab
```

### Step 2

Upload:

```text
Temple_Crowd_Pressure_Dataset_20000.xlsx
```

### Step 3

Run the notebook cells sequentially.

### Step 4

The model will:

```text
Load Dataset
      ↓
Clean Data
      ↓
Train Model
      ↓
Evaluate Model
      ↓
Predict Crowd Pressure
      ↓
Generate Risk Level
```

---

## 🔮 Future Scope

The project can be further improved by:

* Real-time CCTV camera integration
* Real-time crowd counting
* Computer Vision-based density detection
* IoT sensor integration
* GPS-based crowd monitoring
* Live dashboard
* Mobile emergency alerts
* Real-time prediction
* Geographic heatmaps
* Automated emergency notifications
* Integration with smart city systems

---

## ⚠️ Disclaimer

This project is an academic Machine Learning prototype. Its predictions should not be treated as a certified real-world safety or emergency-management system without appropriate validation, domain expertise, operational testing, and safety procedures.

---

## 👨‍💻 Developer

**Mayur Pawar**

M.Sc. Computer Science

MIT Arts, Commerce and Science College

---

## 📜 Project Type

```text
Machine Learning Project
Regression + Classification
Crowd Safety Prediction
Data Science
Python
```

---

## ⭐ Conclusion

The **Temple and Religious Gathering Crowd Stampede Pressure Index Prediction** project demonstrates how Machine Learning can be applied to crowd-flow data to estimate crowd pressure and categorize potential risk levels.

By analyzing crowd, environmental, and event-related factors, the system provides a data-driven prediction that can support further research and the development of intelligent crowd-management systems.
