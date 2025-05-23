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
- **First Fixation Duration**: Duration of the very first fixation.

---

## 🔧 Models & Accuracy

![alt text](image.png)

---

| 🧪 Voting Classifier (LR, SVM, RF)             | 🔢 Accuracy (%) | 📝 Precision (Class 1) | 🔁 Recall (Class 1) | 🎯 F1-Score (Class 1) |
| ---------------------------- | --------------- | ---------------------- | ------------------- | --------------------- |
| ⏱️ Average Fixation Duration | **92.86**       | 1.00                   | 0.86                | 0.92                  |
| 📍 First Fixation Duration   | **85.71**       | 1.00                   | 0.71                | 0.83                  |
| 📊 Number of Fixations       | **57.14**       | 0.60                   | 0.43                | 0.50                  |

---

## 📊 Model Accuracy Comparison
| Model                          | Avg. Fixation Duration Accuracy (%) | Number of Fixation Accuracy (%) | First Fixation Duration Accuracy (%) |
| ------------------------------ | ----------------------------------- | ------------------------------- | ------------------------------------ |
| Logistic Regression            | 81.43                               | 70.00                           | 68.57                                |
| SVM                            | 78.57                               | 61.43                           | 67.14                                |
| Random Forest                  | 71.43                               | 77.14                           | 75.71                                |
| Ridge Classifier               | 64.29                               | 61.43                           | 68.57                                |
| Feature-selected Logistic Reg. | 82.86                               | 75.71                           | 75.71                                |
| MLP (lr=0.05)                  | 82.86                               | 55.71                           | 77.14                                |
| MLP (lr=0.1)                   | 77.14                               | 68.57                           | 75.71                                |
| MLP (lr=0.2)                   | 67.14                               | 61.43                           | 65.71                                |
| kNN (k=1)                      | 64.29                               | 67.14                           | 54.29                                |
| kNN (k=3)                      | 62.86                               | 60.00                           | 54.29                                |
| kNN (k=5)                      | 64.29                               | 60.00                           | 57.14                                |


###






## 💾 Model Output

- Model saved as: `voting_classifier_dyslexia.pkl`

---



