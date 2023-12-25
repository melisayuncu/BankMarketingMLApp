Introduction

The main goal of this project is to create a machine learning model that can predict whether a 
customer will subscribe to term deposits. The project aims to analyze and model the results of 
direct marketing campaigns carried out by a Portuguese banking institution, using the Bank 
Marketing Dataset, specifically the “bankadditional.csv” file, which contains 10% of randomly 
selected samples (4119 samples) from the entire dataset. The project covers data cleaning, 
preprocessing, feature selection, model selection, hyperparameter tuning, and model 
evaluation.

Procedure

First of all, missing values in both categorical and numerical columns were addressed using 
appropriate techniques. Numerical values were imputed with the mode, while categorical values 
were imputed with One-Hot Encoding and Label Encoding methods. In the Data preprocessing 
section, One-Hot Encoding, categorical columns were one-hot encoded to represent them as 
binary values (0 or 1). This step was crucial for transforming categorical variables into a format 
suitable for analysis with the machine learning models. Label Encoding, categorical columns 
were label encoded to represent them as numerical values (such as 0, 1 or 2) while preserving 
their categorical nature. Mode imputation, the mode was used for imputing missing values in 
numerical columns, maintaining the integrity of numerical data.
As the next step, Grid Search were used for Feature selection. The machine automatically 
selected the best features for model training and optimized feature selection based on evaluation 
metrics. Grid Search was used to automatically select the best hyperparameters for each model, 
providing an optimized model for term deposit subscription prediction. This technique 
considered various combinations of features to determine the most effective ones. Moreover, 
L1 & L2 regularization was used as a feature selection method, emphasizing sparsity and 
feature elimination for Logistic Regression model. In the end, calculating Mean AUC values 
for models, the best model which is Logistic Regression was selected. In addition, the pipeline 
of our model is created by using the selected model. Finally, our model is ready to be used in 
the deployment.

The culmination of the project was deploying the final model using Streamlit and creating a 
user-friendly web interface. This interface allows easy interaction with the predictive model, 
making it accessible and practical for end users. The Streamlit cloud address of the deployed 
model is: https://bankmarketingmlapp-jdqxda7zpddexfnt8xazkf.streamlit.app/

Recommendations and Conclusion

In summary, the project successfully developed a predictive model for term deposit subscription 
using machine learning techniques. The selected model showed superior performance after 
comprehensive evaluation. Ongoing maintenance and improvement recommendations include 
periodic retraining with new data and monitoring for changes in dataset distribution. 
As a results, this project represents a comprehensive approach to predictive modeling, from 
data cleansing to distribution. The combination of careful analysis, model selection and user-friendly deployment positions the developed model as a valuable tool for making informed 
decisions in the context of direct marketing campaigns for term deposit subscriptions.
