# 🛡️ Phishing Website Detection Using Machine Learning

## 📘 Overview

This project focuses on detecting phishing websites using **machine learning algorithms**. By analyzing URL-based and content-based features, the system classifies websites as *legitimate* or *phishing*.
The approach combines multiple classifiers such as **Random Forest**, **Decision Tree**, and **Logistic Regression** into a hybrid **Voting Ensemble** model for improved accuracy and robustness.

---

## 📊 Dataset

* **File Name:** `dataset.csv`
* **Source:** UCI Machine Learning Repository – [Phishing Websites Dataset](https://archive.ics.uci.edu/ml/datasets/phishing+websites)
* **Description:** Contains URL-based features such as domain length, presence of “@”, SSL status, prefix/suffix usage, and more.
* **Target Variable:** `Result` (1 = Legitimate, -1 = Phishing)

---

## 🧠 Algorithms Used

1. **Decision Tree Classifier**
2. **Random Forest Classifier**
3. **Logistic Regression**
4. **Voting Ensemble Classifier** (combination of all above)

---

## ⚙️ Implementation Steps

### 1. Data Preprocessing

* Load dataset using `pandas`
* Handle missing values and encode categorical data
* Normalize numerical features for model compatibility

### 2. Model Training and Evaluation

* Split data into **train** and **test** sets (80-20)
* Train all base models individually
* Build a **VotingClassifier** for ensemble prediction
* Evaluate models using:

  * Accuracy
  * Precision
  * Recall
  * F1 Score
  * Confusion Matrix

### 3. Visualization

* Plot accuracy comparison across models
* Display confusion matrix heatmaps for each model

---

## 🧩 Technologies Used

| Component   | Technology                                                 |
| ----------- | ---------------------------------------------------------- |
| Programming | Python                                                     |
| Environment | Google Colab                                               |
| Libraries   | `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn` |

---

## 📈 Sample Results

| Model                      | Accuracy |
| -------------------------- | -------- |
| Decision Tree              | 95.8%    |
| Random Forest              | 97.3%    |
| Logistic Regression        | 95.1%    |
| Voting Ensemble (Proposed) | 98.6%    |

---

## 🚀 How to Run

1. Open the Google Colab notebook (`Phishing_Detection.ipynb`).
2. Upload the dataset (`dataset.csv`) to the Colab environment.
3. Run all the code cells sequentially.
4. Observe model outputs and evaluation results.

---


## 👨‍💻 Author

**Name:** B. Vishnuvardan
**Roll No:** 160123737034
**Course:** Cyber Security

---

## 📚 References

1. Mohammad, R., Thabtah, F., & McCluskey, L. (2015). *Phishing Websites Dataset*, UCI Machine Learning Repository.
2. *Phishing Website Detection using Machine Learning Algorithms*, IEEE, 2022.
3. [Scikit-learn Documentation](https://scikit-learn.org/)
4. [Google Colab](https://colab.research.google.com/)
