# Titanic_Logistic_Regression
# Survival Prediction Project

## Project Intro

This project aims to predict the survival of Titanic passengers based on various factors such as gender, passenger class, age, fare, and more. Using machine learning models like Logistic Regression, the goal is to derive meaningful insights and build a model that can accurately predict whether a passenger survived the disaster.

## Analysis Summary

We explored various factors that influenced the survival of passengers and found several key insights:

- **Gender and Class Impact on Survival**: 
    - Females had a significantly higher survival rate, especially in third class.
    - Higher class passengers (first class) had a better chance of survival than those in second or third class.
    - ![Gender and Class Impact]([https://github.com/gursimran8/Titanic_Logistic_Regression/blob/main/Images/Barplot_gender~class~survival.png)])

- **Model Performance**: 
    - The Logistic Regression model achieved an accuracy of 81%, performing better at predicting non-survivors than survivors.
    - Precision for non-survivors was high at 0.88, while it was slightly lower for survivors (0.70), showing a slight imbalance in predictions.
    - ![Classification Report]([path/to/your/image.png](https://github.com/gursimran8/Titanic_Logistic_Regression/blob/main/Images/Classification%20Report.png))

- **Confusion Matrix**: 
    - The model correctly predicted 92 non-survivors and 52 survivors but misclassified 22 non-survivors and 13 survivors.
    - ![Confusion Matrix]([path/to/your/image.png](https://github.com/gursimran8/Titanic_Logistic_Regression/blob/main/Images/Confusion%20Matrix.png))

- **Correlation Analysis**: 
    - There was a strong negative correlation between gender and survival, with females having a better chance of survival.
    - The fare had a positive correlation with survival, meaning passengers who paid more were more likely to survive.
    - ![Correlation Heatmap]([path/to/your/image.png](https://github.com/gursimran8/Titanic_Logistic_Regression/blob/main/Images/Correlation%20after%20label_encoding.png))

## Problems Faced During Model Creation

1. **Data Imbalance**:
    - The dataset had more non-survivors than survivors, leading to the model being biased toward predicting non-survivors more accurately.

2. **Multicollinearity**:
    - Some features, like `pclass` and `fare`, showed a moderate degree of multicollinearity, impacting the model’s predictive power.

3. **Model Convergence Issues**:
    - Logistic Regression took longer to converge, requiring an increase in the maximum number of iterations (`max_iter`).

## Resolutions

2. **Handling Multicollinearity**:
    - Careful feature selection was applied, and interactions between key features like `pclass` and `fare` were explored to reduce redundancy.

3. **Model Convergence**:
    - We increased the `max_iter` parameter to 1000 for Logistic Regression, ensuring that the model had enough iterations to converge without underfitting.

## Project Outcome

The Logistic Regression model achieved an overall accuracy of 81%, with strong performance in predicting non-survivors. However, by addressing data imbalance and enhancing feature engineering, the model’s ability to predict survivors was improved. The project also highlighted key factors such as gender and class that heavily influenced survival outcomes. The analysis and model creation process provided valuable insights into feature importance and model optimization techniques.


