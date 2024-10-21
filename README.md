
# Fraud Detection Model

This project involves building a fraud detection system using machine learning techniques. The dataset used consists of financial transaction data, including information on fraud and non-fraud cases. The objective is to predict whether a transaction is fraudulent or not.

## Dataset

The dataset contains the following columns:

- **trans_date_trans_time**: Transaction timestamp
- **cc_num**: Credit card number
- **merchant**: Merchant name
- **category**: Category of the transaction
- **amt**: Transaction amount
- **first**, **last**: First and last name of the cardholder
- **gender**, **street**, **city**, **state**, **zip**: Demographic details
- **lat**, **long**, **city_pop**: Geographical location and city population
- **job**, **dob**: Cardholder’s job and date of birth
- **trans_num**: Transaction ID
- **unix_time**: Unix timestamp of the transaction
- **merch_lat**, **merch_long**: Merchant's location
- **is_fraud**: Target variable (1 = Fraud, 0 = Not Fraud)

## Model Training and Evaluation

The project employs several machine learning models to classify transactions:

1. **Logistic Regression**
2. **K-Nearest Neighbors (KNN)**
3. **Decision Tree**
4. **Support Vector Machine (SVM)**

### Preprocessing

- The dataset is split into fraudulent (`is_fraud=1`) and non-fraudulent (`is_fraud=0`) transactions.
- The non-fraudulent data is downsampled to balance the classes.
- Categorical features are encoded using **LabelEncoder**, and numeric columns are scaled using **StandardScaler**.

### Model Performance

After training the models, the following accuracy scores were obtained:

- **Logistic Regression**: XX.XX%
- **K-Nearest Neighbors (KNN)**: XX.XX%
- **Decision Tree**: XX.XX%
- **Support Vector Machine (SVM)**: XX.XX%

Each model’s performance is evaluated using accuracy scores and classification reports to assess precision, recall, and F1-score.

### Visualization

A bar plot showing the new distribution of fraudulent and non-fraudulent transactions after balancing is created using **Seaborn**.

![Fraud Distribution](link-to-plot)

## How to Run

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/fraud-detection.git
    ```
2. Install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the Jupyter notebook or the Python scripts to train and evaluate the models.

## Conclusion

This project demonstrates the effectiveness of various machine learning techniques in detecting fraudulent transactions. The models can be further optimized with hyperparameter tuning and advanced feature engineering.
