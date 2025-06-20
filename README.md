#  Regression Machine Learning with Galaxy

This project showcases my work on building a **regression model** with open source [Galaxy](https://galaxyproject.org/). 

---

## **Objectives**

- Use Galaxy’s visual interface to build a regression model.
- Predict a numerical target variable (e.g., Chronological age).
- Evaluate the model using RMSE, MAE, R², and scatter plots.

---

## ⚙️ Tools & Techniques

---
## **Results**

### **Linear regression performance**

![linreg True vs predicted values](https://github.com/harishmuh/Regression_Machine-Learning-Galaxy/blob/main/docs/linreg_true_pred_curves.png?raw=true)

![linreg residual plot](https://github.com/harishmuh/Regression_Machine-Learning-Galaxy/blob/main/docs/linreg_residual_plot.png?raw=true)

![linreg scatter plot](https://github.com/harishmuh/Regression_Machine-Learning-Galaxy/blob/main/docs/linreg_true_vs_pred_scatter.png?raw=true)

---

### **Ensemble performance: Gradient boosting**

![Gradboost true vs predicted values](https://github.com/harishmuh/Regression_Machine-Learning-Galaxy/blob/main/docs/Gradboost_true_vs_predicted_values.png?raw=true)

![Gradboost residual plot](https://github.com/harishmuh/Regression_Machine-Learning-Galaxy/blob/main/docs/Gradboost_residual%20plot.png?raw=true)

![Gradboost scatter plot](https://github.com/harishmuh/Regression_Machine-Learning-Galaxy/blob/main/docs/linreg_true_vs_pred_scatter.png?raw=true)

---

### **Tuned gradient boosting performance**

![Tuned gb true vs predicted values](https://github.com/harishmuh/Regression_Machine-Learning-Galaxy/blob/main/docs/tunedGB_true_vs_predicted_values.png?raw=true)

![Tuned gb residual plot](https://github.com/harishmuh/Regression_Machine-Learning-Galaxy/blob/main/docs/tunedGB_residualplot.png?raw=true)

![Tuned scatter plot](https://github.com/harishmuh/Regression_Machine-Learning-Galaxy/blob/main/docs/tunedGB_scatterplot.png?raw=true)

---

### **Result summary**

| Model                          | R² Score | RMSE    | Notes                                          |
|--------------------------------|----------|-------|-----------------------------------------------|
| Linear Regression              | 0.93     | 4.10  | Good performance, but could be improved       |
| Gradient Boosting Regressor    | 0.93     | 3.85  | Better RMSE, more robust to outliers          |
| Tuned Gradient Boosting (n=75) | 0.94     | 3.74  | Best performance after hyperparameter tuning  |

---

## **Assets**
* **Workflow diagram**
![Workflow diagram](https://github.com/harishmuh/Regression_Machine-Learning-Galaxy/blob/main/docs/Workflow_diagram.PNG?raw=true)

* **Analysis**
