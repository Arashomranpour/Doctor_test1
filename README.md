<div align="center">

# 🧑‍⚕️ Doctor Assistant - Symptoms to Disease & Advice

**Predict a likely disease from symptoms, then look up its description, precautions, medications, diet and workout suggestions.**

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-337AB7)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white)

</div>

---

![Project screenshot](https://github.com/user-attachments/assets/a40972bb-766b-4139-afe5-e7a6c28bb60a)

## ✨ Overview

An SVM model predicts the disease from a set of symptoms. The predicted disease is then used to recommend, from the CSV lookup tables in `datasets/`:

| Output | Source file |
|---|---|
| 📖 Description | `description.csv` |
| 🛡️ Precautions | `precautions_df.csv` |
| 💊 Medications | `medications.csv` |
| 🥗 Diets | `diets.csv` |
| 🏋️ Workout | `workout_df.csv` |

The notebook (`model.ipynb`) trains and compares top classifiers (**SVC, Random Forest, Gradient Boosting, KNN, Multinomial NB, XGBoost**) on the pre-processed `Training.csv`, and saves the best one as `svc.pkl`.

> ⚠️ Educational project - not medical advice. Consult a doctor.

## 🚀 Getting Started

```bash
git clone https://github.com/Arashomranpour/Doctor_test1.git
cd Doctor_test1
pip install pandas numpy scikit-learn xgboost jupyter
jupyter notebook model.ipynb
```

## 📁 Project Structure

```
.
├── model.ipynb     # Training, comparison, recommendation helpers
├── svc.pkl         # Trained SVM model
└── datasets/       # Training data + description, precautions, medications, diets, workouts, symptom severity
```

## 🛠️ Tech Stack

`scikit-learn` · `XGBoost` · `pandas` · `NumPy`
