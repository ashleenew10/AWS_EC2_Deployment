# CHLA No-Show Predictor – AWS EC2 Streamlit Deployment

This project is a deployed machine learning application that predicts patient no-shows at CHLA clinics using appointment data. The app is hosted on an AWS EC2 instance and built with Streamlit for an interactive frontend.

## 🛠 Technologies Used

- Python 3.12
- Streamlit 1.32.0
- scikit-learn 1.4.2
- pandas 2.2.2
- numpy 1.26.4
- joblib 1.4.2
- AWS EC2 (Ubuntu 22.04)

## How to Run the App on EC2

1. **SSH into your EC2 instance**
   ```bash
   ssh -i "your-key.pem" ubuntu@your-ec2-ip
Clone the GitHub repository

bash
Copy
Edit
git clone https://github.com/ashleenew10/AWS_EC2_Deployment.git
cd AWS_EC2_Deployment
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Launch the Streamlit app

bash
Copy
Edit
streamlit run end_user_app_CHLA.py
Access the app Open the public URL shown in your terminal (port 8501) in a web browser.

Files Included
end_user_app_CHLA.py – Streamlit app script

new_best_no_show_model.pkl – Trained classifier saved with joblib

NEW_no_show_encoder.pkl – Encoders for categorical features

NEW_CLEAN_CHLA_clean_data_2024_Appointments.csv – Cleaned 2024 CHLA data

requirements.txt – Dependency list for the environment

Key Features
Predicts the likelihood of a patient no-show

Allows filtering by clinic and appointment date range

Outputs a confidence score for each prediction

Fully deployed on an AWS EC2 instance using open-source tools


---
