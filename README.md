# 🚀 Meta-Learning-based Traffic Classification for IoT Devices

**👨‍💻 Author:** Saeid Rajabi  
**📧 Email:** [srajabi@udel.edu](mailto:srajabi@udel.edu)  
**🎓 University of Delaware**

---

## 📚 Overview

This project introduces an innovative machine learning framework designed to classify IoT network traffic into benign and various attack types using Meta-Learning techniques. By combining Logistic Regression, Decision Trees, Random Forests, and a Multi-Layer Perceptron (MLP) as a meta-learner, the system achieves remarkable accuracy in both binary and multiclass classification.

---

## 🎯 Objective

To enhance IoT security by accurately detecting and classifying network traffic, thereby preventing sophisticated cyber threats like Mirai and Bashlite (Gafgyt) botnets.

---

## 🗃️ Dataset

- **Dataset:** [N-baiot—network-based detection of IoT botnet attacks using deep autoencoders](https://ieeexplore.ieee.org/abstract/document/8490192?casa_token=WKS579tG4ysAAAAA:PVvXr8WG4WjOLZX8LytucDxhidncXLWjP3l-jMdG9W_UXYuj9R1f9d7hbf8C9crOplfuRjstFw)
- **Devices Included:** Doorbells, thermostats, baby monitors, webcams, and various security cameras.
- **Attack Types Covered:** Mirai (Scan, ACK, SYN, UDP, UDPplain), Bashlite (Scan, Junk, UDP, TCP, COMBO).
- **Features:** 115 statistical features including mean, variance, frequency, and covariance.

---

## 🛠️ Methodology

### 📌 Preprocessing
- Standardization (z-score normalization)
- Synthetic Minority Oversampling Technique (SMOTE) for balancing data
- K-Fold Cross-Validation (K=3)

### 📌 Base Models
- Logistic Regression
- Decision Trees
- Random Forests

### 📌 Meta-Learner
- Multi-Layer Perceptron (MLP)
  - Three hidden layers (32-16-8 neurons)
  - Softmax output layer
  - Dropout (rate=0.2) and L2 regularization

---

## 📊 Results

- **Binary Classification:** Achieved near-perfect accuracy (~100%) in distinguishing benign from attack traffic.
- **Multiclass Classification:** Achieved 88% accuracy overall, with noted challenges particularly in feature overlap between a couple of classes.

---

## 📈 Performance Highlights

- Improved model robustness through meta-learning
- Effective handling of class imbalance and data preprocessing
- Demonstrated capability to learn from noisy and corrupted base model predictions

---

## 🚨 Challenges Encountered

- Class imbalance
- Feature overlap between classes
- Computational limitations during model training

---

## ✨ Future Work

- Explore advanced feature engineering (e.g., autoencoders)
- Experiment with modern architectures (e.g., transformers, graph neural networks)
- Deploy real-time models for live network monitoring
- Implement adversarial training to enhance model robustness

---

## 🛎️ Setup & Execution

- Clone the repository
- Install required libraries (`scikit-learn`, `PyTorch`, etc.)
- Run the provided Jupyter notebooks:
  - `preprocessing.ipynb` for data preprocessing
  - `binary_classification_v1.ipynb` for binary classification
  - `multi_class_code_v1.ipynb` for multiclass classification

---

## 📜 Citation

If you use this work, please cite:

```bibtex
@misc{rajabi2024meta,
  author = {Rajabi, Saeid},
  title = {Meta-Learning-based Traffic Classification for IoT Devices},
  year = {2024},
  publisher = {University of Delaware}
}
```

---

🌟 Feel free to reach out for collaboration or queries!
