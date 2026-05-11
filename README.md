# Task 6: House Price Prediction


## 🎯 Objective
Predict house prices using property features such as size, bedrooms, and location.

## 📊 Dataset
| Property | Details |
|----------|---------|
| Name | Boston Housing Dataset |
| Source | UCI Machine Learning Repository |
| Samples | 506 housing districts |
| Features | 13 property and neighborhood attributes |
| Target | MEDV (Median house value in $1000s) |

### Features Description
| Feature | Description |
|---------|-------------|
| RM | Average number of rooms per dwelling |
| LSTAT | % lower status of the population |
| PTRATIO | Pupil-teacher ratio by town |
| INDUS | Proportion of non-retail business acres |
| NOX | Nitric oxides concentration |
| CRIM | Per capita crime rate by town |
| TAX | Full-value property-tax rate |
| DIS | Weighted distances to employment centers |

## 🔧 Technologies Used
- Python 3.x
- Pandas & NumPy (Data manipulation)
- Scikit-learn (Linear Regression, Gradient Boosting)
- Matplotlib & Seaborn (Visualization)

## 🤖 Models Applied
| Model | MAE ($) | RMSE ($) | R² Score |
|-------|---------|----------|----------|
| Linear Regression | 3,189 | 4,929 | 0.669 |
| Gradient Boosting | 1,941 | 2,708 | 0.900 |

**Best Model:** Gradient Boosting Regressor

## 📈 Key Results & Findings

### Top Important Features (Gradient Boosting)
| Rank | Feature | Importance | Interpretation |
|------|---------|------------|----------------|
| 1 | RM (Avg Rooms) | 47.6% | More rooms = Higher price |
| 2 | LSTAT (Lower Status %) | 32.6% | Higher % = Lower price |
| 3 | DIS (Distance to jobs) | 7.5% | Further from jobs = Lower price |
| 4 | CRIM (Crime rate) | 2.6% | Higher crime = Lower price |

### Model Performance
- **Best MAE:** $1,941 (Gradient Boosting predicts within ~$2K)
- **Best R²:** 0.900 (90% of price variance explained)
- Gradient Boosting outperforms Linear Regression by 23% in MAE

## 📊 Visualizations Generated
1. Feature correlation heatmap
2. Predicted vs Actual price scatter plots
3. Feature importance bar charts
4. Distribution plots

## 🚀 How to Run

### Option 1: Google Colab (Recommended)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/narmeen-hub/House_Price_Prediction/blob/main/House_Price_Prediction.ipynb)

### Option 2: Local Jupyter
```bash
# Clone repository
git clone https://github.com/narmeen-hub/House_Price_Prediction.git
cd House_Price_Prediction

# Install dependencies
pip install -r requirements.txt

# Launch notebook
jupyter notebook House_Price_Prediction.ipynb
