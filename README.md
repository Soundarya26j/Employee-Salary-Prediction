# 💼 Employee Salary Prediction Web App

This project is a **machine learning-powered web application** built using **Streamlit** that predicts the salary of an employee based on their experience and skillset. The app is designed for ease of use and can be accessed both locally and publicly using **ngrok**.

## 📌 Table of Contents

- [📊 Features](#-features)
- [🧠 Tech Stack](#-tech-stack)
- [📁 Project Structure](#-project-structure)
- [⚙️ Installation & Setup](#️-installation--setup)
- [🚀 How to Use](#-how-to-use)
- [🔍 Model Details](#-model-details)
- [🌐 Deployment](#-deployment)
- [🖼️ Screenshots](#-screenshots)
- [🧑‍💻 Author](#-author)
- [📜 License](#-license)

## 📊 Features

- ✅ Predict employee salary based on experience and other features
- 🧠 ML model trained on real-world data using regression
- 🧾 Interactive and user-friendly UI using Streamlit
- 📈 Live display of predicted results
- 🌐 Accessible from anywhere using ngrok tunneling
- 🛠️ Easy to deploy and extend for more features (e.g. role, skills)

## 🧠 Tech Stack

| Component     | Technology               |
|---------------|---------------------------|
| UI            | Streamlit                |
| Backend       | Python                   |
| Machine Learning | Scikit-learn           |
| Model Storage | Joblib (.pkl model)      |
| Deployment    | ngrok (local → public)   |

## 📁 Project Structure:
employee-salary-predictor/
├── app.py                 # Main Streamlit application file
├── model/
│   └── salary_model.pkl   # Trained machine learning model saved using joblib
├── data/
│   └── salary_data.csv    # (Optional) Dataset used to train the model
├── README.md              # Project documentation
├── requirements.txt       # All required Python libraries
└── .gitignore             # Files/folders to ignore in version control

## ⚙️ Installation & Setup:

### 🔹 Step 1: Clone the repository
git clone https://github.com/yourusername/employee-salary-prediction.git
cd employee-salary-prediction

### 🔹 Step 2: Install dependencies
pip install -r requirements.txt
Or manually:
pip install streamlit scikit-learn pandas joblib pyngrok

🔹 Step 3: Train the model (if not already trained)
python train_model.py
This generates a model.pkl file.

🔹 Step 4: Run the Streamlit app
streamlit run app.py

## 🚀 How to Use:
- Open the app in your browser (usually at http://localhost:8501)
- Input the employee's experience (in years) and other fields
- Click Predict Salary
- View the estimated salary output instantly

## 🔍 Model Details:
- Algorithm: Linear Regression
- Input Features:
- Years of Experience
- (Optional) Job Title, Skills, Degree (can be extended)
- Output: Predicted annual salary in INR/USD
- Training: Scikit-learn pipeline with preprocessing and model fitting
- Storage: Saved using joblib as model.pkl

## 🌐 Deployment:
To make the app publicly accessible using ngrok:

🔸 Install ngrok
pip install pyngrok

🔸 Start Streamlit app (Terminal 1)
streamlit run app.py

🔸 Start ngrok tunnel (Terminal 2)
ngrok http 8501
Copy the generated HTTPS link to access the app publicly.

## 🖼️ Screenshots:

<img width="794" height="711" alt="Screenshot 2025-07-24 144620" src="https://github.com/user-attachments/assets/1b703e63-cab1-4d5d-8a97-1678fd9dd060" />
<img width="817" height="724" alt="Screenshot 2025-07-24 144702" src="https://github.com/user-attachments/assets/35da0c73-3bd5-4ec1-a6b9-359862a39e52" />
<img width="665" height="416" alt="Screenshot 2025-07-24 144937" src="https://github.com/user-attachments/assets/769fb6fb-c74a-497e-9ca6-a561b17a640f" />
<img width="1514" height="676" alt="Screenshot 2025-07-24 144927" src="https://github.com/user-attachments/assets/ad5fe3d7-85b6-403c-a6cc-a5e5aa9e1e1f" />
<img width="646" height="839" alt="Screenshot 2025-07-24 144858" src="https://github.com/user-attachments/assets/d6b863bd-61ee-4ca3-8416-ab2d70500734" />
<img width="936" height="844" alt="Screenshot 2025-07-24 144845" src="https://github.com/user-attachments/assets/62aab626-30f3-4113-a09e-178f92533c74" />
<img width="829" height="647" alt="Screenshot 2025-07-24 144733" src="https://github.com/user-attachments/assets/496a8564-cc70-4261-896d-a1814cf82423" />
<img width="1913" height="970" alt="Screenshot 2025-07-24 165649" src="https://github.com/user-attachments/assets/43981c30-6960-4602-80b5-89b6ee617514" />

## 📌 Future Enhancements:
Add support for job title, domain, and location
Use more advanced ML models like Random Forest or XGBoost
Deploy on platforms like Streamlit Cloud, Render, or Heroku
Add data visualizations using Plotly/Altair

## 🧑‍💻 Author:
Soundarya
🎓 Computer Science and Engineering Specialization in Artificial Intelligence and Machine Learning, Sarala Birla University
🌐 LinkedIn: https://www.linkedin.com/in/soundarya-60b330288/ | GitHub

## 📜 License:
This project is licensed under the MIT License.
