# Breast Cancer Classification using KNN

This project implements a **Breast Cancer Classification** model using **K-Nearest Neighbors (KNN)**.  
The pipeline includes **data preprocessing, class imbalance handling with SMOTE, feature scaling**, and **hyperparameter tuning** using **GridSearchCV** with **Stratified K-Fold Cross Validation**.

---

## 📌 Dataset
- **Dataset:** Breast Cancer Wisconsin Dataset
- **Total Samples:** 569
- **Features:** 30 numerical features
- **Target Variable:** `diagnosis`
  - `0` → Benign (B)
  - `1` → Malignant (M)

---

## 🛠️ Technologies Used
- Python
- Pandas
- Scikit-learn
- Imbalanced-learn (SMOTE)

---

## 🔄 Data Preprocessing
- Dropped non-informative `id` column
- Encoded target labels:
  - `B → 0`
  - `M → 1`
- Handled class imbalance using **SMOTE**
- Standardized features using **StandardScaler**

---

## ⚙️ Model Pipeline
```
SMOTE → StandardScaler → KNN Classifier
```

---

## 🔍 Hyperparameter Tuning
**GridSearchCV** was used to find the best parameters.

**Parameter Grid:**
- `n_neighbors`: 3, 5, 7, 9
- `weights`: uniform, distance
- `metric`: euclidean, manhattan

**Cross-Validation Strategy:**
- Stratified K-Fold (5 splits)
- Shuffle enabled

---

## 📈 Model Performance
- **Best Accuracy:** **96.66%**

---

## 📊 Confusion Matrix
```
[[347  10]
 [  9 203]]
```

---

## 🚀 Conclusion
The KNN classifier combined with **SMOTE and scaling** achieved high accuracy and robust performance while handling class imbalance effectively.

---

## 👤 Author
**Zaid**  
BS Computer Science  
Aspiring Machine Learning Engineer
