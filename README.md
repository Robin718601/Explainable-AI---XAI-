# Network Intrusion Detection System using Machine Learning (Random Forest + SHAP)

This project implements a **Network Intrusion Detection System (NIDS)** using the **KDD Cup 99 (NSL-KDD) dataset**.  
A **Random Forest classifier** is trained to detect whether a network connection is **normal** or an **attack**, and **SHAP (SHapley Additive exPlanations)** is used to explain model predictions.

The goal of this project is not only high accuracy, but also **model interpretability**, which is critical in cybersecurity applications.

---

## 🚀 Project Highlights

- Binary classification: **Normal vs Attack**
- Uses **Random Forest** for robust performance
- Handles categorical features using **Label Encoding**
- Visualizes results using:
  - Confusion Matrix
  - Feature Correlation Heatmap
  - SHAP Summary Plot for explainability
- Beginner-friendly but aligned with **real-world cybersecurity use cases**

---

## 📂 Dataset

- **NSL-KDD Dataset**
  - `KDDTrain+.txt`
  - `KDDTest+.txt`

Each record represents a network connection with **41 features** describing traffic behavior.

Target label:
- `0` → Normal
- `1` → Attack

---

## 🧠 Technologies Used

- **Python**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **SHAP**

---

## 🏗️ Project Workflow

1. Load training and testing datasets
2. Assign column names and clean data
3. Convert labels to binary format
4. Encode categorical features:
   - `protocol_type`
   - `service`
   - `flag`
5. Split data into train and test sets
6. Train Random Forest model
7. Evaluate model performance
8. Visualize results
9. Explain predictions using SHAP

---

## 📊 Model Performance

- **Algorithm:** Random Forest Classifier
- **Evaluation Metrics:**
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion Matrix

The model achieves **high accuracy** and performs well in detecting attack traffic.

---

## 📈 Visualizations

- Confusion Matrix Heatmap
- Feature Correlation Heatmap
- SHAP Summary Plot (Top influential features)

SHAP helps understand **why** the model classifies traffic as an attack or normal, which is crucial for security systems.

---

## ▶️ How to Run the Project

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/network-intrusion-detection.git
cd network-intrusion-detection
