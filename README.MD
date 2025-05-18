## ETDD-70 Dataset ( Oct’22 - Aug’23 ) - Czech Language

### Participant : 
- Dyslexia - 35 participants (19 F and 16 M)
- Non-dyslexic - 35 participants (19 F and 16 M)

### Eye to screen distance - 60-70 cm.
### Sampling rate - 250 Hz.

# Dyslexia Detection using Eye-Tracking Data

A machine learning project that uses fixation-based eye-tracking features to detect dyslexia.

[Dataset Link](https://zenodo.org/records/13332134)

---

## 📁 Dataset Description

- **Number of Fixations**: Total fixation count per word.
- **Average Fixation Duration**: Time spent per fixation.

---

## 🔧 Models & Accuracy

---

### ⏱️ Average Fixation Duration – Model Accuracies

**Best SVM Params**: `{'C': 10, 'gamma': 'scale', 'kernel': 'rbf'}`  
**Best SVM Accuracy**: **85.71%**

#### 🔹 MLP and kNN (5-Fold CV)

| Model         | Accuracy (%) |
|---------------|--------------|
| MLP (lr=0.05) | 82.86        |
| MLP (lr=0.1)  | 77.14        |
| MLP (lr=0.2)  | 67.14        |
| kNN (k=1)     | 64.29        |
| kNN (k=3)     | 62.86        |
| kNN (k=5)     | 64.29        |

#### 🔹 Classic ML Models

| Model                             | Accuracy (%) |
|----------------------------------|--------------|
| Logistic Regression              | 81.43        |
| SVM                              | 78.57        |
| Random Forest                    | 71.43        |
| Ridge Classifier                 | 64.29        |
| Feature-selected Logistic Reg.   | 82.86        |

---

### 📊 Number of Fixations – Model Accuracies

**Best SVM Params**: `{'C': 0.1, 'gamma': 'auto', 'kernel': 'rbf'}`  
**Best SVM Accuracy**: **80.00%**

#### 🔹 Classic ML Models

| Model                             | Accuracy (%) |
|----------------------------------|--------------|
| Logistic Regression              | 70.00        |
| SVM                              | 61.43        |
| Random Forest                    | 77.14        |
| Ridge Classifier                 | 61.43        |
| Feature-selected Logistic Reg.   | 75.71        |

#### 🔹 MLP and kNN (5-Fold CV)

| Model         | Accuracy (%) |
|---------------|--------------|
| MLP (lr=0.05) | 55.71        |
| MLP (lr=0.1)  | 68.57        |
| MLP (lr=0.2)  | 61.43        |
| kNN (k=1)     | 67.14        |
| kNN (k=3)     | 60.00        |
| kNN (k=5)     | 60.00        |

---

## 💾 Model Output

- Model saved as: `voting_classifier_dyslexia.pkl`

---



