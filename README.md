# 🧠 BizCred — Credit Score Predictor for Small Businesses

## 📊 Overview  
**BizCred** is a **machine learning-based creditworthiness prediction system** designed for **Micro, Small, and Medium Enterprises (MSMEs)** that often lack formal credit histories.  
By analyzing financial and behavioral indicators, BizCred predicts a **CIBIL-like credit score**, helping lenders assess risk and unregistered businesses gain access to formal credit.

---

## 🚀 Key Features
- 💡 Predicts creditworthiness using **Machine Learning** (Linear Regression & Random Forest).  
- 🧾 Uses **realistic financial & transactional features** as input.  
- 🌐 Interactive **Streamlit web app** for easy access and visualization.  
- 🗃️ **MongoDB integration** for storing user data and prediction history.  
- 📈 User-friendly UI/UX with clear visualization of model outputs.

---

## 🧰 Tech Stack
| Layer | Technology |
|-------|-------------|
| **Frontend** | Streamlit |
| **Backend / ML** | Python, pandas, scikit-learn |
| **Database** | MongoDB |
| **Model Algorithms** | Linear Regression, Random Forest Regressor |
| **Visualization** | Matplotlib, Seaborn |
| **Version Control** | Git, GitHub |

---

## ⚙️ How It Works
1. **Data Input:**  
   Users input key financial and business parameters (e.g., annual income, loan amount, repayment history, etc.).  
2. **Data Preprocessing:**  
   Input is cleaned and standardized for model compatibility.  
3. **Model Prediction:**  
   The trained ML model predicts a **credit score (300–900)**.  
4. **Result Display:**  
   The predicted score and credit risk category (Low, Medium, High) are displayed on the Streamlit interface.  
5. **Database Logging:**  
   All predictions are saved in MongoDB for later review and analytics.

---

## 🧩 Project Structure
BizCred/
│
├── data/
│ └── dataset.csv # Input dataset
│
├── models/
│ ├── linear_regression_model.pkl
│ └── random_forest_model.pkl
│
├── app/
│ ├── main.py # Streamlit app entry point
│ ├── utils.py # Helper functions
│ └── database.py # MongoDB connection script
│
├── notebooks/
│ └── model_training.ipynb # Model training and evaluation notebook
│
├── requirements.txt
├── README.md
└── LICENSE

---

## 💻 Installation & Setup

1️⃣ Clone the Repository
bash
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

###📈 Model Performance
| Metric   | Linear Regression | Random Forest |
| -------- | ----------------- | ------------- |
| R² Score | 0.82              | 0.91          |
| MAE      | 32.5              | 18.3          |
| RMSE     | 45.7              | 23.1          |

###🧑‍💻 Contributors
Yash Nikam – Machine Learning Engineer & UI/UX Developer
Army Institute of Technology, Pune
Under the guidance of Dr. Ashwini Sapkal and Rupali Bagate
