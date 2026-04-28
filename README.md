# Medical_Recomendation_System
Medicine Recommendation System
A machine learning powered web application that predicts diseases based on user symptoms and recommends medications, diets, precautions, and workouts through an interactive health dashboard.

Project Overview
This application allows users to input symptoms and receive:

Predicted disease
Recommended medications
Suggested diet plans
Precautions
Workout recommendations
The system uses machine learning models trained on a medical dataset containing multiple diseases and symptoms.


Dataset Information
The system is trained on a medical dataset containing:

Dataset Component	Count
Total Diseases	57
Total Symptoms	132
Classification Type	Multiclass

Machine Learning Models
Multiple machine learning models were evaluated for disease prediction.

Model	Accuracy
Support Vector Classifier	95.56%
Random Forest	97.3%
Gradient Boosting	72.9%
K-Nearest Neighbors	95.6%
Multinomial Naive Bayes	97.2%
Random Forest and Multinomial Naive Bayes achieved the highest accuracy.


Tech Stack
Backend
Python
Flask
Scikit-learn
Pandas
NumPy
Frontend
React
Vite
TailwindCSS
Recharts
Zustand (state management)
Machine Learning
Scikit-learn
Multiclass classification
Pickle model deployment

Project Structure
Medicine-Recommendation-System
│
├── backend
│   ├── main.py
│   ├── model.pkl
│   ├── requirements.txt
│   └── datasets
│       ├── description.csv
│       ├── diets.csv
│       ├── medications.csv
│       ├── precautions_df.csv
│       ├── Symptom-severity.csv
│       ├── symtoms_df.csv
│       ├── Training.csv
│       └── workout_df.csv
│
└── frontend
    └── health-dashboard
        ├── public
        └── src
            ├── assets
            ├── components
            ├── hooks
            ├── pages
            └── store

How the System Works
User enters symptoms in the dashboard.
The frontend sends a request to the backend API.
The backend loads the trained ML model.
Symptoms are encoded and passed to the model.
The model predicts the most likely disease.
The system retrieves recommendations from datasets.
Results are displayed in the dashboard.

Installation Guide
Clone the Repository
git clone https://github.com/Yash-Bandal/medicine-recommendation-system.git
cd medicine-recommendation-system

Backend Setup
cd backend
pip install -r requirements.txt
python main.py
Backend runs on:

http://127.0.0.1:5000

# or - check main.py

http://127.0.0.1:10000

Frontend Setup
cd frontend/health-dashboard
npm install
npm run dev
Frontend runs on:

http://localhost:5173

License
This project is licensed under the MIT License.
