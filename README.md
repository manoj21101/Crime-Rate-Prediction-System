# Crime-Rate-Prediction-System
**Project Summary: Predicting Crime Victims in India**

**Introduction:**
This project aims to predict the number of crime victims in various age groups across different states in India. The prediction is based on historical crime data, including information about the area, year, and victim demographics. The predictive model utilizes Ridge regression, a machine learning technique, to forecast the number of victims for a given state and year.

**Dataset:**
The dataset used for this project is sourced from Indian crime records and includes information about murder victims categorized by age, gender, area, and year. The dataset spans from 2001 to 2010, providing valuable insights into crime trends over the past decade. The dataset is preprocessed to handle missing values and prepare it for model training.

**Methodology:**
1. **Data Preprocessing:** Missing values in the dataset are filled with zeros, and the data is divided into features (X) and target variables (y). Categorical variables such as 'Area_Name' are one-hot encoded, while numerical variables like 'Year' are scaled using StandardScaler.
  
2. **Model Training:** The preprocessed data is split into training and testing sets. A Ridge regression model is trained using a pipeline that includes preprocessing steps and the Ridge estimator.

3. **Hyperparameter Tuning:** GridSearchCV is employed to tune the hyperparameter alpha for the Ridge regression model. The optimal alpha value is selected based on the mean squared error.

4. **Model Evaluation:** The best-performing model is evaluated using metrics such as Root Mean Squared Error (RMSE), R-squared (R2) score, and Mean Absolute Error (MAE). These metrics assess the accuracy and performance of the model in predicting crime victims.

**Prediction Interface:**
The project provides an interactive interface for users to make predictions based on a selected state and year. Using widgets, users can input a state and a year within the range of 2011 to 2020. The model then predicts the number of crime victims for various age groups in the specified state and year. Additionally, a bar chart visualization is displayed to illustrate the predicted number of victims across different age categories.

**Recommendation:**
For accurate predictions, it is recommended to input years between 2011 and 2020, as the model's training data covers the period from 2001 to 2010. Predictions for years outside this range may not reflect current crime trends accurately.

**Conclusion:**
This project demonstrates the application of machine learning techniques to predict crime victims based on historical data. By leveraging Ridge regression and interactive prediction tools, stakeholders can gain insights into crime patterns and make informed decisions to address public safety concerns in various states of India.
