# Credit-Card-fraud-Prediction

## Problem Statement:
A credit card is one of the most used financial products to make online purchases and payments. Though the Credit cards can be a convenient way to manage your finances, they can also be risky. Credit card fraud is the unauthorized use of someone else's credit card or credit card information to make purchases or withdraw cash.
It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase. 
The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
We have to build a classification model to predict whether a transaction is fraudulent or not.

### Credit card fraud encompasses a range of unauthorized activities undertaken to gain financial advantage by illegally accessing cardholder information. While skimming, the duplication of magnetic strip data, is a prevalent method, other tactics include:

* **Manipulation or alteration of legitimate cards:** Fraudsters may alter existing cards to bypass security measures or encode stolen data.
* **Counterfeit card creation:** Criminals may produce entirely fake cards using stolen information or fictitious details.
* **Exploiting lost or stolen cards:** Lost or stolen cards present an opportunity for unauthorized use.

**Fraudulent telemarketing**, where individuals attempt to obtain card details through deceptive phone calls, is another technique.

**Key improvements:**

* **Formal language:** Replaces informal terms like "dishonest act" with "unauthorized activities."
* **Active voice:** Uses active voice for a more assertive tone ("encompasses" instead of "is").
* **Specificity:** Provides specifics about manipulation/alteration and counterfeit card creation.
* **Conciseness:** Combines "stolen/lost" into "lost or stolen" for brevity.
* **Terminology:** Uses "fraudulent telemarketing" for a more precise term.
* **Structure:** Organizes information into a bulleted list for clarity.

This revised statement conveys the information about credit card fraud in a professional, clear, and informative manner.

## Tasks/Activities List 

- **Data Understanding:** Here, we need to load the data and understand the features present in it. This would help us choose the features that we will need for your final model.
- **Exploratory data analytics (EDA):** Normally, in this step, we need to perform univariate and bivariate analyses of the data, followed by feature transformations, if necessary. For the current data set, because Gaussian variables are used, we do not need to perform Z-scaling. However, you can check if there is any skewness in the data and try to mitigate it, as it might cause problems during the model-building phase.
- **Train/Test Split:** Now we are familiar with the train/test split, which we can perform in order to check the performance of our models with unseen data. Here, for validation, we can use the k-fold cross-validation method. We need to choose an appropriate k value so that the minority class is correctly represented in the test folds.
- **Model-Building/Hyperparameter Tuning:** This is the final step at which we can try different models and fine-tune their hyperparameters until we get the desired level of performance on the given dataset. We should try and see if we get a better model by the various sampling techniques.
- **Model Evaluation:** We need to evaluate the models using appropriate evaluation metrics. Note that since the data is imbalanced it is is more important to identify which are fraudulent transactions accurately than the non-fraudulent. We need to choose an appropriate evaluation metric which reflects this business goal.
