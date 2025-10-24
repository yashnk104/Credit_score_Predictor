🧠 BizCred — Credit Score Predictor for Small Businesses
📊 Overview

BizCred is a machine learning-based creditworthiness prediction system designed for Micro, Small, and Medium Enterprises (MSMEs) that often lack formal credit histories.
By analyzing financial and behavioral indicators, BizCred predicts a CIBIL-like credit score, helping lenders assess risk and unregistered businesses gain access to formal credit.

🚀 Key Features

💡 Predicts creditworthiness using Machine Learning (Linear Regression & Random Forest).

🧾 Uses realistic financial & transactional features as input.

🌐 Interactive Streamlit web app for easy access and visualization.

🗃️ MongoDB integration for storing user data and prediction history.

📈 User-friendly UI/UX with clear visualization of model outputs.

🧰 Tech Stack
Layer	Technology
Frontend	Streamlit
Backend / ML	Python, pandas, scikit-learn
Database	MongoDB
Model Algorithms	Linear Regression, Random Forest Regressor
Visualization	Matplotlib, Seaborn
Version Control	Git, GitHub
⚙️ How It Works

Data Input:
Users input key financial and business parameters (e.g., annual income, loan amount, repayment history, etc.).

Data Preprocessing:
Input is cleaned and standardized for model compatibility.

Model Prediction:
The trained ML model predicts a credit score (300–900).

Result Display:
The predicted score and credit risk category (Low, Medium, High) are displayed on the Streamlit interface.

Database Logging:
All predictions are saved in MongoDB for later review and analytics.

🧩 Project Structure
BizCred/
│
├── data/
│   └── dataset.csv                 # Input dataset
│
├── models/
│   ├── linear_regression_model.pkl
│   └── random_forest_model.pkl
│
├── app/
│   ├── main.py                     # Streamlit app entry point
│   ├── utils.py                    # Helper functions
│   └── database.py                 # MongoDB connection script
│
├── notebooks/
│   └── model_training.ipynb        # Model training and evaluation notebook
│
├── requirements.txt
├── README.md
└── LICENSE

💻 Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/yourusername/bizcred.git
cd bizcred

2️⃣ Create a Virtual Environment
python -m venv venv
source venv/bin/activate    # For Linux/Mac
venv\Scripts\activate       # For Windows

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Run the Streamlit App
streamlit run app/main.py

🧮 Sample Input Features
Feature	Description
Annual Income	Yearly income of the business
Loan Amount	Requested loan amount
Repayment History	Ratio of timely repayments
Business Age	Number of years since establishment
Transaction Volume	Monthly transaction volume
Outstanding Debt	Current unpaid loan amount
Credit Utilization	Credit used vs. available credit
🎯 Output

Predicted Credit Score (e.g., 720)

Credit Risk Category:

🟢 Low Risk (Score ≥ 750)

🟡 Medium Risk (650–749)

🔴 High Risk (Below 650)

📈 Model Performance
Metric	Linear Regression	Random Forest
R² Score	0.82	0.91
MAE	32.5	18.3
RMSE	45.7	23.1

The Random Forest model was selected as the final model due to superior accuracy and robustness.

🧑‍💻 Contributors

Yash Nikam – Machine Learning Engineer & UI/UX Developer
Army Institute of Technology, Pune
Under the guidance of Dr. Ashwini Sapkal and Rupali Bagate

📜 License

This project is licensed under the MIT License — you’re free to use, modify, and distribute with attribution.

🌟 Future Enhancements

Integration with real-time financial APIs (e.g., Razorpay, QuickBooks).

Adding Explainable AI (XAI) for model transparency.

Implementing Credit Report Generation (PDF).

Deployment on AWS / Heroku for public access
