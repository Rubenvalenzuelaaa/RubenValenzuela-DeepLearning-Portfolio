# L08 — Hyperparameter Tuning (SVC Pipeline)

This project demonstrates advanced hyperparameter tuning techniques using Support Vector Machines (SVC) on the Breast Cancer Wisconsin dataset.  
The workflow includes randomized search, grid search, custom ROC/Confusion Matrix plots, learning curves, validation curves, and artifact saving.

---

## 📂 Included Files
- `L08_AIAlchemists_BenjaminLaCount_ITAI2376.pdf`
- Code results extracted from the Jupyter notebook output
- Saved model artifacts (`joblib`)
- Randomized and grid search CSV reports

---

## 🔑 Key Topics
- Support Vector Classifier (SVC)
- Hyperparameter tuning (RandomizedSearchCV + GridSearchCV)
- Log-space sampling for C and gamma
- Learning curves & validation curves
- ROC AUC evaluation and confusion matrix visualization
- Model saving & reproducibility

---

## 🧠 What the Model Does
The SVC classifier predicts whether a breast tumor is **malignant** or **benign** based on 30 numerical features such as:
- mean radius  
- mean texture  
- concavity  
- fractal dimension  
*(see dataset preview in the PDF)*

---

## ⚙️ Methods Used

### **1. Baseline Model**
- Pipeline: `StandardScaler + SVC`
- Cross-validation accuracy: **0.9692 ± 0.0146**
- Test accuracy: **0.9825**
- ROC AUC: **0.9950**

### **2. Randomized Search**
Sampled hyperparameters:
- `C`: log-space between 10⁻¹ and 10²  
- `gamma`: log-space between 10⁻⁴ and 10⁻¹  
- Best params found:
  - `C ≈ 81.05`
  - `gamma ≈ 0.000523`

### **3. Grid Search (fine tuning around best)**
- Best params:
  - `C ≈ 174.62`
  - `gamma ≈ 0.000243`
- Best CV accuracy: **0.9780**

### **4. Tuned Model Results**
- Test accuracy: **0.9825**
- ROC AUC: **0.9940**
- Nearly identical to baseline (dataset is easy + baseline was already near-optimal)

---

## 📊 Visualizations Included
- Baseline ROC curve  
- Tuned model ROC curve  
- Confusion Matrix  
- Learning Curve  
- Validation Curves for:
  - C values (10⁻³ to 10³)
  - gamma values (10⁻⁴ to 10¹)

---

## 🗂️ Saved Artifacts
The code saves:

