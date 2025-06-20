#  **Predicting human chronological age from DNA methylation using supervised regression models with Galaxy**


## **Context**

DNA methylation changes with age at specific [CpG sites](https://en.wikipedia.org/wiki/CpG_site). These changes can act as 'biomarkers' for age prediction, and machine learning models can be trained to estimate age from such methylation features.

In this project, I applied machine learning regression techniques to predict human chronological age based on DNA methylation patterns with open source [Galaxy](https://galaxyproject.org/). 

### **Objectives**

The objectives of this project consisted of:
- To build and compare machine learning regression models using the Galaxy platform.
- To evaluate model performance using standard regression metrics such as R² and RMSE.
- To apply hyperparameter tuning using cross-validation for improving model accuracy.

### **Dataset**

The dataset used in this analysis contains:
- 208 training samples with 13 CpG features and age labels.
- 104 test samples, where models predict age.
- True age values for the test samples are used to evaluate performance.

### **Methods**

I implemented and compared three regression models:
- Linear Regression
- Gradient Boosting Regressor
- Tuned Gradient Boosting Regressor (via hyperparameter tuning)

The regression model performance was assessed using metrics such as:
- R² (coefficient of determination): The closer it is to 1.0, the better it is. If it is negative, then the trained model is not good. 
- RMSE (Root Mean Squared Error): The lower the number, the better it is.


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

### **Insights**
- The linear regression model was able to capture the general trend well, but it had the highest error (RMSE).
- An Ensemble method, like Gradient Boosting, has better performance than basic linear regression and is more robust to outliers.
- Hyperparameter tuning  of the gradient boosting was effective and necessary to optimize model performance, as we see a higher R2 score and a lower RMSE than other models.



## **Conclusion**
This project demonstrates that DNA methylation features can be effectively used to predict human age through machine learning regression models.

* Linear Regression: Provided a strong baseline with good predictive accuracy.
* Gradient Boosting Regressor: Improved performance over linear regression. 
* Tuned Gradient Boosting Regressor: Hyperparameter tuning further enhanced the model performance, achieving the best R² score (0.94) and the lowest RMSE (3.74).

## **Reference**
* [Naue et al., 2017](https://www.sciencedirect.com/science/article/pii/S1872497317301643?via%3Dihub)

## **Assets**
* Workflow diagram
  
![Workflow diagram](https://github.com/harishmuh/Regression_Machine-Learning-Galaxy/blob/main/docs/Workflow_diagram.PNG?raw=true)

* [My Analysis in Galaxy](https://usegalaxy.eu/u/harish_muh12/h/regression-dna-methylation)
