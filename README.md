
🌾 AI-Based Crop Recommendation System






A Machine Learning-powered web application that recommends the most suitable crop based on soil nutrients and climatic conditions.

This project demonstrates an end-to-end ML pipeline including:

Exploratory Data Analysis

Model comparison

Hyperparameter tuning

Feature importance analysis

Model deployment using Streamlit

📌 Problem Statement

Selecting the right crop based on soil and environmental conditions is critical for maximizing agricultural productivity. Traditional decision-making often relies on experience rather than data-driven insights.

This project builds a supervised machine learning model that predicts the most suitable crop using soil nutrients and climate parameters.

📊 Dataset Overview

Total Samples: 2200

Features: 7

Target Classes: Multiple crop categories

Balanced dataset

Input Features:

Nitrogen (N)

Phosphorus (P)

Potassium (K)

Temperature (°C)

Humidity (%)

pH

Rainfall (mm)

Target Variable:

Crop Label

🔎 Exploratory Data Analysis (EDA)

Comprehensive analysis was performed to understand feature distribution and relationships.

1️⃣ Nutrient Analysis by Crop

Insight: Different crops require significantly different nitrogen levels.

<img width="1389" height="590" alt="Average Nitrogen content for each crop" src="https://github.com/user-attachments/assets/c73cea72-2138-4ecc-847d-566346750987" />


2️⃣ Rainfall Distribution

Insight: Rainfall is one of the strongest differentiators among crops.

<img width="1389" height="590" alt="Rainfall Distribution across Crops" src="https://github.com/user-attachments/assets/fd5f5b8c-f66f-4d28-aafe-7dabed1ff534" />


3️⃣ Correlation Heatmap

Insight:

Low multicollinearity

Features largely independent

<img width="892" height="789" alt="Feature Correlation Matrix" src="https://github.com/user-attachments/assets/3e1ee6d2-af65-41ea-b0c0-5eab559706db" />

4️⃣ Feature Importance (Random Forest)

Top Influential Features:

Rainfall

Humidity

Potassium (K)

<img width="794" height="659" alt="Feature Importance Distribution" src="https://github.com/user-attachments/assets/3bf0f931-247e-4b06-9654-394c6775334e" />

🤖 Model Development
Models Evaluated:

Logistic Regression

Decision Tree

Random Forest

Support Vector Machine

🏆 Final Model: Random Forest Classifier
📈 Performance:

Accuracy: ~98–99%

Cross-validation applied

Stable performance across folds

High class-level precision & recall

Why Random Forest?

Handles non-linear relationships well

Robust against overfitting

Provides interpretable feature importance

🌐 Web Application (Streamlit)

The system includes an interactive web interface that allows users to:

Enter soil nutrient values

Provide environmental parameters

Receive real-time crop recommendations

View prediction confidence score

See top 3 suggested crops

Visualize feature importance

<img width="1903" height="862" alt="app_scrnsht_01" src="https://github.com/user-attachments/assets/2c09af95-2111-40ed-b33e-efa6d23c4cf0" />

🛠 Tech Stack

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Streamlit

Joblib

📁 Project Structure
Crop-prediction-project/
  │── app.py
  │── notebook.ipynb
  │── dataset.csv
  │── models/
  │── images/
  │── README.md
  │── requirements.txt
  │── .gitignore

🚀 How to Run
git clone https://github.com/ragunathan0812/Crop-prediction-project.git
cd Crop-prediction-project

conda create -n ds python=3.10
conda activate ds
pip install -r requirements.txt

streamlit run app.py

📌 Future Improvements

Fertilizer recommendation module

Crop yield prediction

Real-time weather API integration

Cloud deployment (Streamlit Cloud / Render)

👨‍💻 Author

Ragunathan
Machine Learning & Data Science Enthusiast
