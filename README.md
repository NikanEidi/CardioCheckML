# 🫀 CardioCheckML

**CardioCheckML** is a machine learning project that predicts the **risk of heart attack** based on key medical indicators. It is built using a dataset of 303 patient records and applies various classification algorithms to determine whether a patient is at **high risk** or **low risk** of heart disease.

---

## 📊 Dataset Features

The dataset includes the following medical attributes:

- `age`: Age of the patient
- `sex`: Gender (0 = female, 1 = male)
- `cp`: Chest pain type (0–3)
- `trtbps`: Resting blood pressure (in mm Hg)
- `chol`: Cholesterol level in mg/dl
- `fbs`: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)
- `restecg`: Resting electrocardiographic results (0–2)
- `thalachh`: Maximum heart rate achieved
- `exng`: Exercise-induced angina (1 = yes, 0 = no)
- `oldpeak`: ST depression induced by exercise
- `slp`: Slope of the peak exercise ST segment
- `caa`: Number of major vessels (0–4) colored by fluoroscopy
- `thall`: Thalassemia (0–3)
- `output`: Target variable (0 = low risk, 1 = high risk)

---

## ⚙️ Project Steps

1. **Data Loading & Exploration**
   - Used `pandas`, `matplotlib`, and `seaborn` for exploration.
   - Checked for missing/null values and data types.
   - Used a heatmap to visualize feature correlation.

2. **Feature Selection & Scaling**
   - Selected the most relevant features based on correlation.
   - Applied `StandardScaler` for feature normalization.

3. **Model Training**
   - Tried multiple classification models:
     - Logistic Regression  *(Best accuracy)*
     - Random Forest
     - Decision Tree
     - K-Nearest Neighbors (KNN)
     - Support Vector Machine (SVM)

4. **Model Evaluation**
   - Evaluated using:
     - Accuracy Score
     - Confusion Matrix
     - Classification Report
     - ROC Curve

---

## 🧠 Best Performing Model

**Logistic Regression** showed the highest accuracy on the test set:

- **Accuracy**: ~88.5%
- **Precision/Recall**: Balanced performance across both classes.
- Evaluated with ROC Curve and heatmap-based feature importance.

---

## 📁 Files

- `heart.csv`: The dataset used
- `CardioCheckML.ipynb`: Main Jupyter Notebook
- `heart_model.pkl`: Saved trained model (for further use)
- `scaler.pkl`: Saved `StandardScaler` object

---
