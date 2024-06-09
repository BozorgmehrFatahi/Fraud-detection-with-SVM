# Fraud-detection-with-SVM
# Fraud Detection Model

This code trains a fraud detection model using the Support Vector Machines (SVM) algorithm. The model is trained on a dataset of fraudulent and non-fraudulent transactions to predict the likelihood of fraud in new transactions.

## Data Preprocessing

The training data is read from a CSV file and outliers are removed from each column for non-fraudulent transactions using the Interquartile Range (IQR) method.

## Model Training

The SVM algorithm is used for training the model, and hyperparameter tuning is performed using Randomized Search Cross Validation to find the best hyperparameters for the model. The hyperparameters considered for tuning are 'C' (regularization parameter), 'gamma' (kernel coefficient), and 'kernel' (kernel type).

The training data is split into input features (
X
) and the target variable (
y
). The best hyperparameters obtained from Randomized Search CV are used to create an SVM model, which is then trained on the training data.

## Model Evaluation

The trained model is evaluated on a testing set, and the F1 score is used as the performance metric to assess the model's ability to correctly classify fraudulent transactions.