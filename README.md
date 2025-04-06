# 🛡️ A Comparative Study of Machine Learning Models for Ransomware Detection

**Author:** Pratik Bhandari  
**Institution:** Department of Computer Science, San Jose State University  

This project explores the application of various machine learning models to detect ransomware using system feature data. It aims to provide a robust, efficient detection mechanism capable of identifying both known and evolving ransomware threats.

---

## 📄 Abstract

This study presents a machine learning-based approach for ransomware detection using a dataset of system-level features. The solution involves data preprocessing, feature engineering, model training, and evaluation of several algorithms to achieve high detection accuracy and low false positive rates. The results are validated using test data to ensure the system's practical applicability and reliability in dynamic environments.

---

## 🧠 Keywords

`Ransomware Detection` · `Machine Learning` · `Cybersecurity` · `Anomaly Detection` · `Supervised Learning` · `Feature Engineering` · `Data Preprocessing`

---

## 📊 Dataset

The dataset was sourced from [Kaggle](https://www.kaggle.com/datasets/amdj3dax/ransomware-detection-data-set) and includes **62,485 samples** with **18 numerical features** extracted from Portable Executable (PE) headers of files. These features help distinguish between benign and ransomware-infected files.

---

## ⚙️ Methodology

### 🔍 Data Preprocessing
- Removed missing/inconsistent rows
- Dropped string-based and redundant features
- Standardized numeric features with `StandardScaler`
- Applied an 80:20 train-test split with cross-validation

### 🧪 Machine Learning Models
- **Logistic Regression** (with cost-sensitive learning)
- **Support Vector Machines (SVM)** with linear, polynomial, and RBF kernels
- **Random Forest Classifier**

### 📈 Evaluation Metrics
- Accuracy, Precision, Recall, F1-Score
- Confusion Matrices for visual performance analysis

---

## 📌 Results Summary

| Model                | Accuracy | Precision | Recall | F1-Score |
|---------------------|----------|-----------|--------|----------|
| Logistic Regression | 0.87     | 0.91      | 0.77   | 0.84     |
| SVM (RBF Kernel)    | 0.95     | 0.96      | 0.93   | 0.95     |
| Random Forest       | 0.99     | 1.00      | 1.00   | 1.00     |

Random Forest demonstrated the highest accuracy and balance between precision and recall, making it the most effective model in this study.

---

## 📉 Challenges

- Overfitting due to dataset characteristics
- Limited generalizability despite cross-validation
- Need for more diverse data to improve robustness

---

## 🚀 Future Work

- Incorporate additional and more diverse datasets
- Explore advanced validation strategies like nested CV
- Develop a ransomware detection application using pre-trained models

---

## 🧾 Conclusion

This project successfully compared several machine learning models for ransomware detection. While all models performed well, **Random Forest** and **SVM with RBF** stood out in terms of accuracy and F1-score. Despite overfitting concerns, the results are promising for developing scalable ransomware defense tools using machine learning.

---

## 📚 References

1. Chainalysis. *Ransomware hit $1 billion in 2023*. https://www.chainalysis.com/blog/ransomware-2024/  
2. Reed, J. *Ransomware payouts hit all-time high*. https://securityintelligence.com/articles/ransomware-all-time-high-attackers-struggle/  
3. Kaggle. *Ransomware Detection Dataset*. https://www.kaggle.com/datasets/amdj3dax/ransomware-detection-data-set

---

> 💻 *Developed as part of a research project at San Jose State University by [Pratik Bhandari](https://bhprtk.com)*
