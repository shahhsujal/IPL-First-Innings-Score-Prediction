# 🏏 IPL 1st Innings Score Prediction using Machine Learning

## 📌 Overview
This project focuses on predicting the **first innings total** in Indian Premier League (IPL) T20 matches using **machine learning regression models**. The models are trained on historical **ball-by-ball data from 2008 to 2017** and aim to estimate the final first innings score based on features like overs, runs, wickets, and team stats.

Among the models tested, **Random Forest Regressor** performed best with **94.06% test accuracy**, proving to be highly effective for real-time mid-innings score prediction.

---

## 📊 Dataset
- 📁 Source: [Kaggle IPL Dataset](https://www.kaggle.com/yuvrajdagur/ipl-dataset-season-2008-to-2017)
- 🔄 Preprocessing:
  - Removed powerplay overs (1–5)
  - Kept consistent teams only
  - One-hot encoded teams
  - Features: `overs`, `runs`, `wickets`, `runs_last_5`, `wickets_last_5`, team indicators
  - Target: `total` (first innings total)

---

## 🤖 Models Used
- Linear Regression
- Lasso Regression
- Decision Tree Regressor
- **Random Forest Regressor** ✅ *(Best Performer)*
- Support Vector Regressor (SVR)
- Multi-layer Perceptron (Neural Network)

### 📈 Model Evaluation Metrics
| Model                   | Test Accuracy (%) | MAE   | RMSE  |
|------------------------|-------------------|-------|--------|
| Random Forest           | **94.06**         | 4.28  | 7.32   |
| Decision Tree           | 87.30             | 3.76  | 10.71  |
| MLP Regressor (Neural)  | 85.95             | 8.35  | 11.75  |
| Linear Regression       | 67.00             | 12.98 | 17.27  |
| Lasso Regression        | 66.09             | 13.01 | 17.51  |
| SVR                     | 58.55             | 14.60 | 19.36  |

---

## 📈 Visual Analysis
- Correlation heatmaps
- Feature importance from Random Forest
- First innings score distribution
- Model comparison chart (R² test scores)

---

## 🧪 Use Cases (Sample Predictions)
| Overs | Runs | Wickets | Runs (Last 5) | Wickets (Last 5) | Predicted | Actual |
|-------|------|---------|----------------|------------------|-----------|--------|
| 18.0  | 150  | 4       | 57             | 1                | 173       | 172    |
| 14.0  | 118  | 1       | 45             | 0                | 186       | 185    |
| 18.0  | 96   | 8       | 18             | 4                | 108       | 110    |

---

## 🛠️ Tech Stack
- Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
- Jupyter Notebook / Google Colab

---

## ⚠️ Limitations & Future Work
- Limited to IPL data from 2008–2017
- Doesn’t consider toss, venue, player form, or weather
- Future improvements:
  - Live dashboard for predictions
  - More contextual features
  - Use of ensemble stacking or time series modeling

---

## 👨‍💻 Authors
- Shivaan Lalwani
- **Sujal Shah**
- Tejbir Singh Khalsa  
*Department of Information Technology, NMIMS MPSTME*

---

## 📎 Tags
`IPL` `Machine Learning` `Score Prediction` `Regression Models` `Random Forest` `Cricket Analytics`

