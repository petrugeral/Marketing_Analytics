# Marketing Campaign Conversion Prediction Project

## Objective
This project aims to predict which customers converted in the last marketing campaign of a store using machine learning techniques. The main focus is to identify customers most likely to convert, enabling more efficient targeting of marketing strategies.

## Dataset
The dataset used in this project was obtained from Kaggle and includes information about sales, marketing campaigns, and customer data.

### Selected Features
- **Purchase Profile in Percentage Terms:**
  - MntWines_percent
  - MntFruits_percent
  - MntMeatProducts_percent
  - MntFishProducts_percent
  - MntSweetProducts_percent
  - MntGoldProds_percent

- **Buyer Profile in the Face of Recent Marketing Campaigns:**
  - buyer_status
  - buyer_class

- **Gross Volume of Purchases:**
  - MntTotal
  - MntRegularProds

- **Volume of Purchases in Each Channel:**
  - NumDealsPurchases
  - NumWebPurchases
  - NumCatalogPurchases
  - NumStorePurchases

- **Customer Historical Information:**
  - Recency (time since the last purchase)
  - Customer_Days
  - main_channel_Store (if the store is their main channel)
  - NumWebVisitsMonth

- **Age Information:**
  - Age

### Feature Engineering
Techniques such as Principal Component Analysis (PCA), Correlation Matrix, and Random Forest Classifier (Gini coefficient) were applied for feature engineering to reduce the need for features. The final feature selection was based on the importance identified during the feature engineering phase.

## Tested Models
The following machine learning models were tested:
- Logistic Regression
- Support Vector Machine (SVM)
- Random Forest
- XGBoost
- Neural Network

## Selected Model
The chosen model for prediction was **Logistic Regression**. This choice was based on a combination of performance and computational efficiency, as Logistic Regression exhibited high accuracy while maintaining low computational cost.

## Evaluation Metrics
The final model presented the following evaluation metrics:
- Accuracy: 95%
- Recall: 99%
- Precision: 92%

These metrics indicate that the model is capable of identifying the majority of customers who actually converted in the last campaign, minimizing false positives.

## How to Use This Repository
1. **Prerequisites:**
   - Make sure to have the required libraries installed (check the `requirements.txt` file).
  
2. **Repository Structure:**
   - `data/`: Contains the dataset used in the project.
   - `models/`: Stores the trained model.
   - `README.md`: This document.

3. **Instructions for Reproduction:**
   - Execute the notebooks in the order indicated in the `notebooks/` directory.
   - Use the source code in the `src/` directory to train and evaluate the model.
   - The trained model will be saved in the `models/` directory.

4. **Model Parameters:**
   - Model parameters are defined in the `src/model_train.py` file.
   - Modify parameters as needed for experimentation.

## Questions and Contact
For questions or suggestions, contact Giovane Petruccelli at giovanepetruccelli@gmail.com.
