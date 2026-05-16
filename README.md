# 🐶🐱 Cat vs Dog Image Classification using SVM

This project implements a **Support Vector Machine (SVM)** model to classify images of cats and dogs using the Kaggle Cats vs Dogs dataset.

The model uses:
- HOG (Histogram of Oriented Gradients) feature extraction
- SVM classifier with RBF kernel

---

# 🚀 Technologies Used

- Python
- NumPy
- OpenCV
- Scikit-learn
- Matplotlib
- scikit-image

---

# 🧠 Machine Learning Model

Algorithm Used:
- **Support Vector Machine (SVM)**

Kernel:
- **RBF Kernel**

Feature Extraction:
- **HOG (Histogram of Oriented Gradients)**

---

# ⚙️ Project Workflow

1. Load images
2. Preprocess images
3. Extract HOG features
4. Train SVM classifier
5. Perform cross-validation
6. Evaluate model
7. Generate visualizations
8. Save trained model

---

# 📊 Dataset Summary

| Dataset | Cats | Dogs | Total |
|---|---|---|---|
| Training Set | 2000 | 2000 | 4000 |
| Test Set | 1011 | 1012 | 2023 |

---

# 📊 HOG Feature Extraction

Feature Vector Size:

```text
1764
```

---

# 📈 Cross Validation Results

```text
CV Accuracy: 74.20% ± 1.48%
```

---

# 📋 Model Evaluation Results

```text
Test Accuracy : 73.01%
```

---

# 📄 Classification Report

```text
              precision    recall  f1-score   support

         Cat       0.72      0.74      0.73      1011
         Dog       0.74      0.72      0.73      1012

    accuracy                           0.73      2023
   macro avg       0.73      0.73      0.73      2023
weighted avg       0.73      0.73      0.73      2023
```

---

# 📌 Output Files Generated

```text
hog_visualization.png
confusion_matrix.png
precision_recall_chart.png
svm_cat_dog.joblib
```

---

# 💻 Complete Output

```text
==================================================
   SVM Cat vs Dog Classifier
==================================================

[INFO] Loaded 2000 cats + 2000 dogs = 4000 total

[INFO] Loaded 1011 cats + 1012 dogs = 2023 total

[INFO] Extracting HOG features — training set...
Extracting HOG features: 100%|███████| 4000/4000

[INFO] Extracting HOG features — test set...
Extracting HOG features: 100%|███████| 2023/2023

[INFO] HOG feature vector size: 1764

[INFO] Training SVM pipeline (StandardScaler + RBF SVC)...

[INFO] Running 5-fold cross-validation...

[INFO] CV Accuracy: 74.20% ± 1.48%


==================================================
        MODEL EVALUATION RESULTS
==================================================

  Test Accuracy : 73.01%

  Classification Report:
              precision    recall  f1-score   support

         Cat       0.72      0.74      0.73      1011
         Dog       0.74      0.72      0.73      1012

    accuracy                           0.73      2023
   macro avg       0.73      0.73      0.73      2023
weighted avg       0.73      0.73      0.73      2023

```
