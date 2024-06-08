# Table-Classification-from-Financial-Statements-Using-NLP


# Financial Statement Table Classification

This project classifies tables from financial statements into the following categories:
- Income Statements
- Balance Sheets
- Cash Flows
- Notes
- Others

## Dataset

The dataset comprises HTML files that include tabular data. Each subfolder in the dataset corresponds to one of the above categories.

## Approach

### 1. Data Extraction and Preprocessing

#### 1.1. Extraction

The tables are extracted from HTML files using BeautifulSoup and pandas.

#### 1.2. Preprocessing

The extracted tables are cleaned by removing non-alphabetic characters, converting text to lowercase, and removing extra spaces and 'nan' values.

### 2. Feature Extraction
#### 2.1. TF-IDF Vectorization
The text data is vectorized using TF-IDF to convert the textual information into numerical format suitable for model training.

### 3. Model Selection and Training
#### 3.1. Handling Class Imbalance
SMOTE (Synthetic Minority Over-sampling Technique) is applied to address class imbalance in the dataset.

### 3.2. Model Training
An SVM classifier is selected for its effectiveness in text classification tasks. Hyperparameter tuning is performed using GridSearchCV to find the best parameters.

# Results
After training and hyperparameter tuning, the SVM classifier achieved an accuracy of xx% on the test set. This demonstrates the model's capability to classify tables from financial statements into the specified categories effectively.

# Conclusion
The task involved extracting and preprocessing data from HTML files, feature extraction using TF-IDF, handling class imbalance with SMOTE, and training an SVM classifier with hyperparameter tuning. The final model demonstrated satisfactory performance with a high accuracy rate.
