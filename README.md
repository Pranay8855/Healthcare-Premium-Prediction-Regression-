-- Health Insurance Premium Prediction System --
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/68f31b44-aa02-435f-978e-412ad8c0e295" />

#Overview:
The Health Insurance Premium Prediction System is a machine learning-based application designed to estimate insurance premium values based on various demographic, financial, and health-related attributes.

This system analyzes multiple features such as age, income, medical history, lifestyle habits, and family dependencies to predict the premium amount. The model is integrated with a Streamlit web application that allows users to easily input their details and receive real-time premium predictions.

To improve prediction accuracy, the project introduces a model segmentation strategy where separate models are trained for young individuals and other age groups.

#Problem Statement
Health insurance companies determine premium amounts based on various risk factors such as age, health conditions, income level, and lifestyle choices. Traditional estimation methods may not always capture complex relationships between these factors.

This project aims to develop a machine learning model that can accurately predict insurance premium values using multiple relevant features and make the prediction system accessible through an interactive web interface.

#Features Used in Prediction

#The following features are used as input variables for premium prediction:

- Age
- Number of Dependents
- Income (in Lakhs)
- Genetic Risk
- Insurance Plan
- Employment Status
- Gender
- Marital Status
- BMI Category
- Smoking Status
- Region
- Medical History

These attributes help represent both the financial capacity and health risk profile of individuals.

#Project Workflow

1. Data Collection
The dataset used for this project was obtained from the UCI Machine Learning Repository. It contains demographic, financial, and medical attributes related to individuals and their insurance details.

These variables serve as the input features for training the machine learning models used to predict insurance premium values.

2. Feature Engineering
Data preprocessing and feature engineering were performed to prepare the dataset for model training. The steps included:

- Handling missing values
- Encoding categorical variables
- Data transformation
- Feature selection

3. Model Training
Multiple machine learning models were trained using the prepared dataset to predict insurance premium values. The models learned relationships between input features and the premium amount.

4. Model Fine Tuning
Hyperparameter tuning techniques were applied to optimize model performance and improve prediction accuracy.

5. Error Analysis
Model predictions were evaluated to identify prediction errors and performance limitations. This analysis helped in refining the model and improving reliability.

6. Model Segmentation
To enhance prediction accuracy, the dataset was segmented into two groups:

- Young Individuals
- Other Age Groups

Separate models were trained for each segment, enabling the system to better capture age-specific patterns in insurance premium calculations.

7. Artifact Generation
After training, the models and preprocessing components were saved as artifacts using Joblib. These artifacts are used during prediction without retraining the models.

#Examples of artifacts include:

- Trained model files
- Data preprocessing pipelines
- Encoders and transformers

#Streamlit Web Application
A Streamlit-based web interface was developed to allow users to interact with the prediction system.

#The application enables users to:

- Enter personal, financial, and medical details
- Submit the input data
- Receive predicted insurance premium values instantly

This interface makes the system accessible to users without requiring programming knowledge.

#API Integration
The trained machine learning models are connected to the Streamlit application through an API-like interface, enabling real-time predictions based on user input.

#Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Joblib
- Streamlit

