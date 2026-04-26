# 📊 Simple Linear Regression: Height vs Weight

## 📌 Overview

This project demonstrates the implementation of **Simple Linear Regression** to model the relationship between a person's **height** and **weight**.

The goal is to predict a person's weight based on their height using a trained machine learning model.

---

## 🧠 Concept

Simple Linear Regression models the relationship between two variables using a straight line:

[
y = mx + b
]

Where:

* **y** → Dependent variable (Weight)
* **x** → Independent variable (Height)
* **m** → Slope of the line
* **b** → Intercept

---

## 📂 Dataset

* File: `height-weight.csv`
* Features:

  * `Height` (input feature)
  * `Weight` (target variable)

---

## ⚙️ Tech Stack

* Python 🐍
* NumPy
* Pandas
* Matplotlib / Seaborn
* Scikit-learn
* Pickle (for model saving)

---

## 🚀 Workflow

### 1. Data Preprocessing

* Load dataset using Pandas
* Handle missing values (if any)
* Separate features (X) and target (y)

### 2. Feature Scaling

* Applied `StandardScaler` to normalize input data

### 3. Model Training

* Used `LinearRegression` from Scikit-learn
* Trained model on scaled data

### 4. Model Saving

* Saved trained model using `pickle`
* Saved scaler separately for future predictions

### 5. Prediction

* Loaded model and scaler in a separate notebook
* Scaled new input data
* Predicted weight

---

## 📁 Project Structure

```
section29/
│
├── linear_regression.ipynb   # Model training
├── predict.ipynb             # Prediction using saved model
├── height-weight.csv         # Dataset
├── model.pkl                 # Trained model
├── scaler.pkl                # Saved scaler
└── README.md                 # Project documentation
```

---

## 🧪 How to Run

### Step 1: Train the Model

Run:

```
linear_regression.ipynb
```

This will generate:

* `model.pkl`
* `scaler.pkl`

---

### Step 2: Make Predictions

Run:

```
predict.ipynb
```

Modify input:

```python
x_new = [[170]]  # Example height
```

---

## 📈 Example Prediction

Input:

```
Height = 170 cm
```

Output:

```
Predicted Weight ≈ XX kg
```

---

## ⚠️ Important Notes

* Input must match training format (same number of features)
* Always apply scaler before prediction
* Do not skip preprocessing steps

---

## 🔥 Future Improvements

* Add multiple features (age, gender, etc.)
* Deploy model using Flask / FastAPI
* Build a frontend interface

---

## 👨‍💻 Author

Saumya Prakash Narayan
