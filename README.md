# 🌱 Hybrid Renewable Energy Forecasting for Microgrid Applications

This repository presents a hybrid renewable energy forecasting framework designed for **microgrid applications**, integrating both **solar (photovoltaic)** and **wind power forecasting models**.

The work is based on our conference paper:

📄 **T. -C. Ou, Y. -T. Chen and Y. -W. Jhang, "Optimization of hybrid renewable power forecasting model for microgrid applications," 2025 IEEE Industry Applications Society Annual Meeting (IAS), Taipei, Taiwan, 2025, pp. 1-8, doi: 10.1109/IAS62731.2025.11061564.**
👉 

---

## 📌 Project Overview

Due to the intermittency and uncertainty of renewable energy, accurate forecasting is essential for:

* Microgrid energy management
* Storage dispatch optimization
* Grid stability enhancement

This project proposes a **hybrid forecasting framework** combining:

* Deep learning (CNN, BiLSTM, Attention)
* Machine learning (LSSVM)
* Swarm intelligence optimization (BSO)

---

## ⚡ System Structure

The project is divided into two main parts:

### ☀️ Solar Power Forecasting (Photovoltaic) — *My Contribution*

This part focuses on short-term solar power prediction using a deep learning architecture:

* CNN → spatial feature extraction
* BiLSTM → temporal dependency modeling
* Attention → dynamic feature weighting

📊 Model:

```
CNN + BiLSTM + Attention
```

📈 Key Features:

* Captures both spatial and temporal patterns
* Improves forecasting accuracy compared to LSTM/BiLSTM
* Suitable for volatile solar conditions

📌 According to the paper, this model achieved the best performance among all solar models 

---

### 🌬️ Wind Power Forecasting

This part focuses on wind power prediction using machine learning:

* Model: LSSVM (Least Squares Support Vector Machine)
* Optimization: Bee Swarm Optimization (BSO)

📊 Model:

```
LSSVM + BSO
```

📈 Key Features:

* Efficient for nonlinear regression
* Improved generalization via swarm optimization
* Outperforms ARIMAX, RF, and SVR

---

## 📂 Repository Structure

```
├── solar_CNN+BiLSTM.ipynb     # Solar forecasting model (my work)
├── paper.pdf                  # Conference paper
├── data/                      # (optional) dataset
├── results/                   # (optional) figures & outputs
└── README.md
```

---

## 🧠 Methodology

### 1. Data Processing

* Hourly meteorological + power data (Taiwan Datan region)
* Missing value imputation
* Feature selection (Pearson correlation + p-value)
* Seasonal classification & K-means clustering

---

### 2. Solar Forecasting (Deep Learning)

* Input: weather + historical PV power
* Architecture:

  * CNN layers
  * BiLSTM layers
  * Attention mechanism
* Output: predicted PV power

---

### 3. Wind Forecasting (Machine Learning)

* Input: wind-related meteorological features
* Model: LSSVM
* Optimization: BSO for hyperparameters

---

### 4. Evaluation Metrics

* MAE (Mean Absolute Error)
* RMSE (Root Mean Square Error)
* MRE (Mean Relative Error)

These metrics evaluate prediction accuracy and robustness.

---

## 🚀 Results

* Hybrid models outperform traditional methods
* Solar model (CNN + BiLSTM + Attention) shows best accuracy
* Wind model (LSSVM + BSO) improves stability and performance
* Data classification enhances prediction under stable conditions

---

## 🧑‍💻 My Contribution

* Designed and implemented the **solar forecasting model**
* Developed:

  * CNN + BiLSTM + Attention architecture
  * Feature engineering and preprocessing
* Conducted model training and performance evaluation
* Integrated results into the hybrid framework

---

## 📌 Future Work

* Dual-mode forecasting (low/high power regimes)
* Improved robustness under extreme weather
* Integration with real-time microgrid control systems

---

## 📎 Requirements

* Python 3.x
* TensorFlow / Keras
* NumPy, Pandas, Scikit-learn
* Matplotlib

---

## 📬 Contact

Yu-Tung Chen
MSc Student, National Cheng Kung University
📧 [jess1357992@gmail.com](mailto:jess1357992@gmail.com)

---

## ⭐ Citation

If you use this work, please cite:

```
Chen, Y.-T., Ou, T.-C., et al.
Optimization of Hybrid Renewable Power Forecasting Model for Microgrid Applications.
IEEE IAS Annual Meeting, 2025.
```

---

## 📝 License

This project is for academic and research purposes.

---

