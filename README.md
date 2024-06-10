# Credit Card Fraud Prediction

## Problem Statement:
A credit card is one of the most used financial products to make online purchases and payments. Though the Credit cards can be a convenient way to manage your finances, they can also be risky. Credit card fraud is the unauthorized use of someone else's credit card or credit card information to make purchases or withdraw cash.
It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase. 
The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
We have to build a classification model to predict whether a transaction is fraudulent or not.

## Overview
This project aims to build a classification model to predict whether a credit card transaction is fraudulent or not. The dataset contains transactions made by European cardholders in September 2013, and the data is highly imbalanced, with fraudulent transactions accounting for only 0.172% of all transactions.

## Dataset
The dataset used in this project can be accessed [here](https://github.com/charanrajupodila/Credit-Card-fraud-Prediction). It contains 284,807 transactions, with 492 frauds.

## Project Structure
- **Exploratory Data Analysis (EDA)**: Analyze and understand the data to identify patterns and trends.
- **Data Cleaning**: Handle missing values and outliers.
- **Data Balancing**: Address the class imbalance using SMOTE.
- **Feature Engineering**: Create and transform features for better model performance.
- **Model Selection and Training**: Train multiple models (Logistic Regression, Decision Tree, Random Forest, and XGBoost).
- **Model Validation**: Evaluate model performance using metrics like accuracy, precision, recall, F1-score, and ROC AUC.
- **Hyperparameter Tuning**: Optimize the model parameters to improve performance.

## Setup and Installation
1. **Clone the repository**:
    ```sh
    git clone https://github.com/your-username/credit-card-fraud-prediction.git
    cd credit-card-fraud-prediction
    ```

2. **Create a virtual environment**:
    ```sh
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\\Scripts\\activate`
    ```

3. **Install the required packages**:
    ```sh
    pip install -r requirements.txt
    ```

4. **Launch Jupyter Notebook**:
    ```sh
    jupyter notebook
    ```

5. **Open the notebook**:
    Open the `Prediction of Credit Card fraud.ipynb` notebook in Jupyter and run the cells sequentially.

## Usage
1. **Data Loading**: The notebook loads the dataset and performs exploratory data analysis (EDA).
2. **Data Cleaning**: Handles any missing values and outliers.
3. **Data Balancing**: Balances the data using the SMOTE technique.
4. **Model Training**: Trains multiple classification models and evaluates their performance.
5. **Hyperparameter Tuning**: Uses GridSearchCV to find the best hyperparameters for the chosen model.

## Evaluation Metrics
The models are evaluated based on the following metrics:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**
- **ROC AUC**

## Results
The results of the model evaluations and the tuned hyperparameters are documented in the notebook.

## Future Work
- Implement additional data preprocessing techniques.
- Explore other machine learning models and advanced ensemble methods.
- Deploy the model in a production environment for real-time fraud detection.

## Contributing
Feel free to fork the repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License
This project is licensed under the MIT License.

## Tasks/Activities List 

- **Data Understanding:** Here, we need to load the data and understand the features present in it. This would help us choose the features that we will need for your final model.
- **Exploratory data analytics (EDA):** Normally, in this step, we need to perform univariate and bivariate analyses of the data, followed by feature transformations, if necessary. For the current data set, because Gaussian variables are used, we do not need to perform Z-scaling. However, you can check if there is any skewness in the data and try to mitigate it, as it might cause problems during the model-building phase.
- **Train/Test Split:** Now we are familiar with the train/test split, which we can perform in order to check the performance of our models with unseen data. Here, for validation, we can use the k-fold cross-validation method. We need to choose an appropriate k value so that the minority class is correctly represented in the test folds.
- **Model-Building/Hyperparameter Tuning:** This is the final step at which we can try different models and fine-tune their hyperparameters until we get the desired level of performance on the given dataset. We should try and see if we get a better model by the various sampling techniques.
- **Model Evaluation:** We need to evaluate the models using appropriate evaluation metrics. Note that since the data is imbalanced it is is more important to identify which are fraudulent transactions accurately than the non-fraudulent. We need to choose an appropriate evaluation metric which reflects this business goal.
