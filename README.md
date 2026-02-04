## Heart Disease Risk Prediction

This project aims to analyze and understand heart disease risk using real clinical data, following a step-by-step and fully explanatory approach. The main emphasis is not on using automated libraries, but on understanding the process, the data, and the decisions made throughout the analysis.

The work is developed as part of an academic laboratory focused on logistic regression, exploratory data analysis (EDA), and evaluation of predictive model performance.

## Project Objective

The main objectives of this project are:

Analyze a real-world patient dataset

Identify patterns associated with the presence of heart disease

Build a logistic regression model from scratch

Clearly and thoughtfully interpret the obtained results

## Dataset Used

The project uses the Heart Disease Dataset, a well-known dataset that contains clinical information from patients, including:

-Age
-Blood pressure
-Cholesterol
-Maximum heart rate
-Exercise-related and electrocardiographic variables
-A target variable indicating the presence or absence of heart disease

The dataset is stored in the following directory:

data/heart.csv

## Analysis Development

All project development is fully documented and executed within a Jupyter Notebook.

## IMPORTANT NOTE

The Jupyter notebook that contains the complete development is named Feature Selection.
This notebook systematically addresses the following key aspects:

Exploratory Data Analysis (EDA)
Data completeness and missing value verification
Variable preparation and transformation
Logistic regression algorithm convergence
Model performance evaluation
Interpretation of results
Interpretation of model coefficients

## Analysis Content
### 1. Exploratory Data Analysis (EDA)
At this stage, an initial exploration of the dataset is performed in order to:
Understand the structure of the data
Identify the available variable types
Analyze the distribution of the target variable
Verify whether the dataset is balanced
A clear visualization of patients with and without heart disease is included.

<img width="711" height="708" alt="image" src="https://github.com/user-attachments/assets/3f083253-8e5c-48bd-8aa3-b4b609ed9c5b" />

Bar chart showing class distribution (0: absence, 1: presence)

### 2. Data Completeness

The dataset is checked for missing values, confirming that the data is suitable for model training without requiring complex imputation techniques.
This step is essential to ensure the reliability of the subsequent analysis.

### 3. Data Preparation
In this phase, the following steps are performed:
Conversion of the target variable to binary format
Selection of relevant features
Splitting the dataset into training and testing sets (70% / 30%)
Normalization of numerical variables
These steps allow the model to be trained in a stable and consistent manner.

### 4. Model Training
A logistic regression model is implemented from scratch, following the theoretical concepts covered in class:
Sigmoid function
Cost function
Gradient descent algorithm
During training, the convergence of the algorithm is analyzed by observing how the cost decreases across iterations.

<img width="873" height="689" alt="image" src="https://github.com/user-attachments/assets/f2848b6f-74bf-41cb-8e13-e13bc062ed9f" />

Cost vs. iterations plot

### 5. Performance Evaluation

Once trained, the model’s performance is evaluated using the following metrics:
Accuracy
Precision
Recall
F1-score
These metrics are analyzed on both the training and test sets to assess the model’s generalization capability.
### 6. Results Interpretation
An interpretative analysis of the results is conducted, explaining:
How well the model separates patients with and without heart disease
The limitations of the linear decision boundary
The reliability of the predictions produced
### 7. Coefficient Interpretation
Finally, the model coefficients are analyzed to understand:
Which variables have the strongest influence on predictions
How changes in clinical factors affect disease probability
The relationship between medical data and model output
This step connects the mathematical model with the real-world healthcare context.
### Decision Boundary Visualization
<img width="1173" height="335" alt="image" src="https://github.com/user-attachments/assets/982b8348-1fe0-49fa-9f87-695bc9434014" />

To analyze the ability of the logistic regression model to separate classes, models were trained using pairs of features, and their decision boundaries were visualized.

The figure shows three feature combinations:

-Age vs. Cholesterol
-Blood Pressure vs. Maximum Heart Rate
-ST Depression vs. Number of Observed Vessels

Data points represent training and test samples, while the line indicates the decision boundary learned by the model.

## Visual Evidence of Development

Throughout the laboratory development, several visual outputs and notebook executions were generated, including:
Successful notebook execution
Training results
Main analytical plots

## Cloud Deployment Status
The project includes a planned deployment stage using AWS SageMaker.
However, this phase has not yet been completed due to permission restrictions in the current environment.
The project is fully prepared to continue with cloud deployment once full access to the required services is available.

## Conclusion
This project provides a practical and progressive understanding of how to apply logistic regression to a real healthcare problem, emphasizing data interpretation, algorithm behavior, and result explanation rather than simply generating predictions.

## Author

Samuel Antonio Gil Romero
