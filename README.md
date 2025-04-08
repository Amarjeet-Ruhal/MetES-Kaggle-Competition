# MetES Kaggle Competition: Predicting Electrical Conductivity of Alloys

This repository contains the solution for the **MetES Kaggle Competition**, which focuses on predicting the **Electrical Conductivity (%IACS)** of metallurgical alloys based on their chemical composition and processing parameters.

## 🧪 Problem Statement

The task is to build a machine learning model that predicts the electrical conductivity of alloy samples using various metallurgical features including:
- Elemental composition
- Processing conditions
- Mechanical properties

The goal is to **minimize Mean Absolute Error (MAE)** between predicted and actual %IACS values.

## 📁 Dataset

The dataset includes the following columns:

### 🔹 Features:
- **Elemental Composition**: Cu, Al, Ag, B, Be, Ca, Co, Ce, Cr, Fe, Hf, La, Mg, Mn, Mo, Nb, Nd, Ni, P, Pb, Pr, Si, Sn, Ti, V, Zn, Zr
- **Processing Conditions**:
  - `Tss (K)`: Solution treatment temperature
  - `tss (h)`: Solution treatment time
  - `CR reduction (%)`: Cold rolling reduction
  - `Aging`, `Tag (K)`, `tag (h)`: Aging process details
  - `Secondary thermo-mechanical process`
- **Additional Properties**:
  - `Hardness (HV)`
  - `Yield Strength (MPa)`
  - `Ultimate Tensile Strength (MPa)`

### 🎯 Target:
- `Electrical Conductivity (%IACS)`

## ⚙️ Best Model Summary

The best-performing model was **Random Forest Regressor**.

### ✅ Final Parameters:
- `n_estimators`: 325  
- `max_depth`: None  
- `min_samples_split`: 7  
- `min_samples_leaf`: 1  
- `max_features`: 'sqrt'

### 📊 Evaluation Metric:
- **MAE**: 13.61438

## 📈 Other Models Tested
| Model                  | Performance (MAE)     |
|------------------------|------------------------|
| Random Forest (Best)   | **13.61438**           |
| Linear Regression      | **13.69008**           |
| XGBoost                | **13.66300**           |
| Neural Network         | **19.68904**           |

## 🔍 Feature Importance
Key features contributing most to the target prediction:
- **Composition**
- `Tss (K)`
- `tss (h)`
- `CR reduction (%)`
- `Tag (K)`
- `tag (h)`
- `Hardness (HV)`

## 🚀 Future Work
- Try ensembling techniques to further improve performance
- Apply domain-specific feature engineering
- Use polynomial or interaction features
- Hyperparameter tuning via Bayesian Optimization

## 📂 Files
- `train.csv`: Dataset used for training
- `notebook.ipynb`: Code for model development and testing
- `report.pdf` / `report.md`: Detailed analysis and findings
- `README.md`: Project overview

## 🧑‍💻 Author
- [Amarjeet]
- [GitHub](https://github.com/Amarjeet-Ruhal)]

---

Happy Modeling! 🔬⚡
