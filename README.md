📞 Call Drop Prediction with Weather Data

This project builds a machine learning pipeline that predicts whether a phone call will be dropped based on call metadata and weather conditions. It integrates Excel call records with weather history, performs feature engineering, and trains models including XGBoost and Random Forest to evaluate prediction performance.


---

🚀 Features

Data Preprocessing

Cleans and converts Excel and CSV date formats.

Merges call logs with weather data.

Engineers features like call duration thresholds and drop status.


Machine Learning Models

XGBoost with ROC curve and AUC evaluation.

Random Forest with confusion matrix and feature importance plots.


Visualization

ROC curve for XGBoost.

Feature importance plots using randomForest and ggplot2.




---

📂 Project Structure

├── data/
│   ├── Arafat.xlsx              # Call data (input file)
│   ├── weatherHistory.csv       # Weather dataset (input file)
│
├── scripts/
│   └── call_drop_model.R        # Main R script
│
├── README.md                    # Project documentation


---

📦 Requirements

Install the following R packages before running the script:

install.packages(c("dplyr", "readxl", "xgboost", "pROC", 
                   "randomForest", "caret", "ggplot2"))


---

⚙️ Usage

1. Clone this repository

git clone <your-repository-url>
cd call-drop-prediction


2. Place your datasets in the data/ folder:

Arafat.xlsx → Call data file

weatherHistory.csv → Weather dataset



3. Run the R script

source("scripts/call_drop_model.R")




---

📊 Model Outputs

✅ XGBoost

ROC Curve plotted

AUC value printed


✅ Random Forest

Confusion matrix with accuracy, precision, recall

Feature importance plots



---

📈 Example Results

XGBoost AUC: ~0.85 (depends on data)

Random Forest Accuracy: ~80–90% (depends on data)



---

🔮 Next Steps

Hyperparameter tuning for both models.

Try other ML algorithms (SVM, Logistic Regression).

Deploy as an API for real-time prediction.



---

👨‍💻 Author

Developed by Ashish Rajput