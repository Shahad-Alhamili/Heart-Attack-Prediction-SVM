# Heart Attack Prediction Using SVM

This project demonstrates the use of the Support Vector Machine (SVM) algorithm to predict the likelihood of a heart attack based on patient health data. SVM is a powerful supervised machine learning algorithm particularly effective on smaller datasets and complex classification tasks.

---

## Project Overview

Heart disease is one of the leading causes of mortality worldwide. Early prediction and diagnosis can significantly improve patient outcomes. This project builds an SVM-based classifier to predict whether a patient is at risk of a heart attack using key health indicators.

---

## Dataset

- The dataset used contains various patient health metrics, including age, cholesterol level, resting blood pressure, and maximum heart rate.
- Data preprocessing includes handling missing values and selecting relevant features.
- Features used:
  - `age` — Patient age in years
  - `chol` — Serum cholesterol level (mg/dl)
  - `trtbps` — Resting blood pressure (mm Hg)
  - `thalachh` — Maximum heart rate achieved
- Target variable:
  - `output` — Heart attack occurrence (1 = yes, 0 = no)

---

## Methodology

### 1. Import Libraries

Key libraries used for data manipulation, visualization, and modeling:
- `numpy`, `pandas`
- Visualization: `matplotlib`, `seaborn`, `pywaffle`
- Machine learning and preprocessing: `sklearn`

### 2. Data Loading and Preprocessing

- Load the dataset and handle missing or invalid data.
- Split data into training and testing sets.
- Features are standardized using `StandardScaler`.

### 3. Data Visualization

- Waffle chart showing percentage of patients at risk.
- Density plots illustrating distribution of features for normal vs heart attack classes.

### 4. Model Building and Hyperparameter Tuning

- Use `SVC` from `sklearn` for Support Vector Machine classification.
- Perform hyperparameter tuning with Grid Search on kernel type and regularization parameter `C`.
- Best model parameters found: `kernel='linear'`, `C=1`.

### 5. Prediction and Evaluation

- Predict heart attack occurrence on the test set.
- Evaluate the model using:
  - Classification report (precision, recall, f1-score)
  - Confusion matrix (visualized with a heatmap)
- Achieved an accuracy of ~75%.

### 6. Model Testing with New Data

The model is tested with unseen patient inputs to predict the risk of a heart attack.
the model achieved an accuracy of 75 %
![image](https://github.com/user-attachments/assets/a9be520e-ffcc-494d-8f8a-75053512ae3d)


---
## ▶️ How to Run

1. Open the notebook in Google Colab:
   👉 [Open in Colab](https://colab.research.google.com/drive/1ORo6zvPtjpv59vA-zflN9lmDgRwAFnAm#scrollTo=Xcm_UXU9pJGk)
---

## 🪪 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👩‍💻 Author

**Shahad Alhamili**  
AI Student & Engineer  
GitHub: [@Shahad-Alhamili](https://github.com/Shahad-Alhamili)
