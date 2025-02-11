# fraud-detection
Machine learning model for fraud detection in rental transactions
## Dataset
Due to file size limitations, download the dataset from [Google Drive](https://drive.google.com/file/d/1rB7hgMEz2sicxJ-KO7gUzSE5ibNfBgNI/view?usp=sharing).

# Fraud Detection in Rent Payments

## 📌 Problem Statement
Detect fraudulent rental transactions using machine learning models based on transaction data.

## 📂 Dataset
The dataset used is the [Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

## 📁 Repository Structure
fraud-detection/
├── data/
│   └── creditcard.csv (Download separately)
├── notebooks/
│   └── fraud_detection.ipynb  # Jupyter notebook with ML models
├── models/
│   └── best_fraud_detection_model.pkl  # Trained XGBoost model
├── README.md  # Project documentation
└── requirements.txt  # Python dependencies
## Clone the Repository 
To download and set up the project, run:
git clone https://github.com/sabinachou/fraud-detection.git

## Install Dependencies
pip install -r requirements.txt

## 📊 Model Performance
| Model              | Precision | Recall | F1-Score | AUC-ROC |
|--------------------|----------|--------|----------|---------|
| **Logistic Regression** | 0.85 | 0.78 | 0.81 | 0.92 |
| **XGBoost**        | 0.90 | 0.82 | **0.86** | **0.95** |
| **Isolation Forest** | 0.10 | 0.85 | 0.18 | 0.89 |
| **One-Class SVM**  | 0.05 | 0.81 | 0.09 | 0.89 |

**🔹 Best Model:** `XGBoost` achieves the **highest F1-score of 0.86** and **AUC-ROC of 0.95**.

## Future Improvements
Hyperparameter tuning for better fraud detection accuracy.
Testing on additional fraud datasets.
Deploying the model using Flask or FastAPI for real-time fraud detection.

