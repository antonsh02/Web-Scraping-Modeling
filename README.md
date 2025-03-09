# Wikipedia Scraping and Predictive Modeling
#### Overview
This project focuses on **predictive modeling** using WIkipedia data to analyze three key attributes: 
1. **Length** -- Predicting the length of Wikipedia articles.
2. **Word Presence** -- Classifying whether a specific word is present in an article.
3. **Edited in 2023** -- Predicting whether an article was edited in 2023.
   
The pipeline includes **web scraping, data preprocessing, feature engineering, regression, and classification modeling**.

---

## Data Collection & Preprocessing
- Retrieved **training and testing datasets** from Wikipedia links.  
- **Imputed missing values** using a simple imputer (replaced NaNs with the mean).  
- Standardized numerical features using **StandardScaler**.  
- Split data into **80% training and 20% testing**.  
---

## Regression Modeling (Length Prediction)
To predict article length, I evaluated multiple regression models:  
- **Linear Regression**  
- **Lasso Regression**  
- **Ridge Regression**  
- **Random Forest Regressor**  
- **Decision Tree Regressor**  
- **Elastic Net Regression**  
- **MLP Regressor (Neural Network)**  

Models were evaluated using **Mean Absolute Error (MAE)** and R² score.

---

## Classification Modeling (Word Presence & Edit History)
For the **binary classification tasks**, I tested the following models:  
- **Logistic Regression**  
- **Random Forest Classifier**  
- **MLP Classifier (Neural Network)**  

I fine-tuned hyperparameters and assessed model performance using a **confusion matrix** and classification metrics.

---
