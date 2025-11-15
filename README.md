🩺 Liver Function Analysis – Machine Learning Project

This project focuses on predicting liver disease using patient clinical data. A machine learning model is trained using features such as bilirubin levels, enzyme counts, protein metrics, age, and gender. The goal is to classify whether a patient is likely to have liver disease based on their test results.

📌 Project Overview

The dataset contains medical attributes used for liver diagnosis, including:

Age

Gender

Total Bilirubin

Direct Bilirubin

Alkaline Phosphotase

Alamine Aminotransferase (ALT)

Aspartate Aminotransferase (AST)

Total Proteins

Albumin

Albumin/Globulin Ratio

Dataset (Label: 1 = Liver Disease, 2 = No Liver Disease)

This project preprocesses the dataset, trains machine learning models, evaluates accuracy, and predicts the patient class.

🧠 Machine Learning Workflow

Data Cleaning

Handling missing values

Converting categorical columns (Gender)

Removing duplicates

Exploratory Data Analysis (EDA)

Distribution of attributes

Correlation heatmaps

Outlier detection

Feature Engineering

Encoding Gender

Normalizing numeric features

Model Training
Algorithms used:

Logistic Regression

Random Forest

Decision Tree

SVM (optional)

Evaluation

Accuracy Score

Precision, Recall, F1-score

Confusion Matrix

Prediction

Taking new patient values

Predicting disease presence

📂 Project Structure
Liver-Function-Analysis/
│── data/
│   └── liver.csv
│── notebooks/
│   └── analysis.ipynb
│── model/
│   ├── liver_model.pkl
│   └── scaler.pkl
│── src/
│   ├── preprocess.py
│   ├── train.py
│   └── predict.py
│── README.md

⚙️ How to Run
1. Install Dependencies
pip install -r requirements.txt

2. Run Jupyter Notebook
jupyter notebook

3. Train the Model
python src/train.py

4. Make Predictions
python src/predict.py

🧪 Sample Input
{
  "Age": 65,
  "Gender": "Female",
  "Total_Bilirubin": 0.7,
  "Direct_Bilirubin": 0.1,
  "Alkaline_Phosphotase": 187,
  "Alamine_Aminotransferase": 16,
  "Aspartate_Aminotransferase": 18,
  "Total_Protiens": 6.8,
  "Albumin": 3.3,
  "Albumin_and_Globulin_Ratio": 0.9
}

Sample Output
{
  "prediction": "Liver Disease"
}

📈 Results

Achieved 84% accuracy using the best-performing model.

Random Forest / Decision Tree usually performs best for this dataset.

👨‍💻 Developer

Ruksana – Machine Learning & Data Analysis
