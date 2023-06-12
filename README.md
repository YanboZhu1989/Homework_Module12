# Homework_Module12
## Loan Status Prediction

### Data Preprocessing
The lending_data.csv file is loaded from the Resources folder into a Pandas DataFrame. The DataFrame is then separated into labels (y) and features (X). The label set (y) is created from the “loan_status” column, and the features (X) DataFrame is created from the remaining columns. After that, the balance of the labels variable (y) is checked using the value_counts function. Finally, the data is split into training and testing datasets using train_test_split.

### Model Training
A logistic regression model is fit using the training data (X_train and y_train). The LogisticRegression module from SKLearn is imported for this purpose.

### Model Evaluation
The model's performance is evaluated by calculating the accuracy score, generating a confusion matrix, and printing the classification report.

### Model Prediction
The predictions on the testing data labels are saved using the testing feature data (X_test) and the fitted model. The model is able to predict both healthy loans (0 label) and high-risk loans (1 label) quite accurately.

### Model Training with Resampled Data
The model's performance with the resampled data is evaluated by calculating the accuracy score, generating a confusion matrix, and printing the classification report.

### Model Prediction with Resampled Data
The model predictions are then made using the resampled data. 
The logistic regression model with oversampled data performs well for both healthy loans and high-risk loans, demonstrating improved recall for high-risk loans.
