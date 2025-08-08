# ELab_Task4

# 🧮 Logistic Regression - Binary Classification
 
The objective is to build a **binary classification model** using Logistic Regression, evaluate it with multiple metrics, and fine-tune the decision threshold for optimal results.

---

## 📌 Objective

Train and evaluate a Logistic Regression model on a binary dataset to:
- Predict class labels based on feature inputs.
- Analyze performance with metrics like precision, recall, F1-score, and ROC-AUC.
- Tune decision thresholds for improved results.

---

## 🛠️ Tools & Libraries Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn

---

## 📂 Dataset

The dataset used is the **Breast Cancer Wisconsin Dataset**, loaded from `sklearn.datasets`.  
**Target Variable:**  
- `0` → Malignant  
- `1` → Benign  

**Features:**  
30 numerical features describing cell nucleus measurements.

---

## 📊 Project Process

### 1. Data Loading & Preprocessing
- Loaded dataset from `sklearn.datasets`.
- Checked shape, column names, and missing values.
- Standardized features using `StandardScaler`.

### 2. Model Training
- Split data into training and testing sets (80-20 split with stratification).
- Trained Logistic Regression model (`solver='liblinear'`).

### 3. Evaluation Metrics
- Confusion Matrix  
- Precision, Recall, F1-score  
- ROC Curve and ROC-AUC score  
- Precision–Recall Curve

### 4. Threshold Tuning
- Adjusted decision threshold to maximize F1-score.
- Compared default (0.5) vs tuned threshold performance.

### 5. Handling Class Imbalance
- Used `class_weight='balanced'` if imbalance was present.

---

## 📈 Key Insights
- Logistic Regression performed with high ROC-AUC (~0.99).
- Threshold tuning improved the balance between precision and recall.
- Visualizations like ROC and PR curves helped interpret model performance.

---

## 📁 Files in Repository

| File Name                        | Description                                      |
|----------------------------------|--------------------------------------------------|
| `ElevateLabs_Task4.ipynb`        | Full code and visualizations for the project     |
| `data.csv`                       | Dataset                                          |
| `README.md`                      | Project documentation (this file)                |

---


## 🙌 Acknowledgements

- Dataset from [Scikit-learn](https://scikit-learn.org/stable/datasets.html)

