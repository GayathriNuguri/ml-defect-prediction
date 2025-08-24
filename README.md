Defect Prediction using Machine Learning

This project focuses on predicting software defects using classical Machine Learning models.
The dataset used is defect_dataset-ant-1.3.csv (software defect dataset).
The workflow covers data preprocessing, feature engineering, model training, evaluation, and best model identification.

Project Structure

ml-defect-prediction/
│
├── data/
│   └── defect_dataset-ant-1.3.csv     # dataset (optional, may be ignored in .gitignore)
│
├── notebooks/
│   └── Defect_Prediction.ipynb        # main notebook with code + outputs
│
├── results/
│   ├── baseline_metrics.png            # chart comparing baseline models
│   ├── tuned_metrics.png               # chart comparing tuned models
│   ├── best_model_summary.md           # explanation of the best model
│   └── Defect_Prediction.html          # HTML export of the notebook
│
├── requirements.txt                    # dependencies
├── README.md                           # project documentation
└── .gitignore                          # ignored files

🚀 Workflow

Data Preprocessing

Checked and handled missing values

Capped outliers at 1st and 99th percentiles

Corrected skewness with log transformation

Standardized numerical features

Feature Engineering

Correlation analysis with target (bug)

Removed low-correlation and redundant features

Applied scaling for distance-based models (KNN, Logistic Regression)

Model Training

Logistic Regression

Decision Tree

K-Nearest Neighbour

Random Forest (Ensemble)

Class Imbalance Handling

Used SMOTE to oversample the minority class

Model Evaluation

Metrics: Accuracy, Precision, Recall, F1-score, AUC-ROC

Compared baseline vs tuned models

Hyperparameter tuning with Stratified K-Fold Cross Validation

📊 Results

Baseline Models: Logistic Regression, Decision Tree, KNN, Random Forest

Tuned Models: Hyperparameter tuning improved performance (esp. Random Forest)

Best Model: Random Forest (highest Accuracy, Precision, Recall, F1-score, and AUC-ROC)

Setup :
# Create virtual environment
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows

# Install dependencies
pip install -r requirements.txt

Notes

No deep learning models are used — only classical ML.

All outputs are included in the notebook and HTML export.

Due to small dataset size, results (esp. perfect metrics) should be interpreted with caution.
