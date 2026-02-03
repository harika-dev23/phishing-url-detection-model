# Phishing URL Detection Model

## Overview
- This project is a **Machine Learning–based Phishing URL Detection System** that analyzes URLs and classifies them as **Phishing** or **Legitimate**.  
- The system extracts multiple lexical, domain-based, and content-based features from URLs and applies a **Random Forest classifier** to detect phishing attempts.

- The solution includes a **Flask web application** that allows users to check single URLs or upload a file containing multiple URLs for batch detection.

## Problem Statement
- Phishing attacks exploit deceptive URLs to steal sensitive information. Traditional rule-based detection is limited and ineffective against evolving attack patterns.  
- This project automates phishing detection by leveraging **feature engineering and machine learning** techniques.

## System Architecture
- User Input (URL / File Upload)
- Feature Extraction (30+ URL features)
- Machine Learning Model (Random Forest)
- Flask Backend API
- Prediction: Phishing / Legitimate

## Tech Stack
- **Language:** Python  
- **Machine Learning:** Scikit-learn (Random Forest)  
- **Backend:** Flask  
- **Data Processing:** NumPy  
- **Frontend:** HTML, Bootstrap, jQuery  
- **Libraries:** BeautifulSoup, Requests, Whois  

## Project Structure
- feature_extraction.py # URL feature extraction logic
- phishing_detection.py # Model training & prediction
- server.py # Flask application
- dataset.csv # Training dataset
- Features.txt # Feature definitions
- getInput.html # Web UI
- URL.txt # Sample URLs
- README.md # Documentation

## Feature Engineering
The system extracts **30 different features** from each URL, including:
- IP address presence  
- URL length and shortening services  
- SSL certificate status  
- Domain registration age  
- DNS records  
- Web traffic and page rank  
- Suspicious HTML behaviors (iframes, popups, mouseover scripts)

These features are used to train the ML model for classification.

## Machine Learning Model
- **Algorithm:** Random Forest Classifier  
- **Train/Test Split:** 80/20  
- **Input:** URL feature vector  
- **Output:**  
  - `Phishing URL`  
  - `Legitimate URL`

The model is trained dynamically and used for real-time prediction.

## Web Application Features
- Detect phishing for a **single URL**
- Upload a **file containing multiple URLs**
- Displays prediction results instantly
- Simple and user-friendly interface

## How to Run the Project
## 1. Install Dependencies
- pip install flask numpy scikit-learn beautifulsoup4 requests python-whois googlesearch-python
## 2. Run the Application
- python server.py
## 3. Access the App
- http://localhost:

## Results & Impact
- Successfully classifies phishing and legitimate URLs
- Demonstrates strong feature engineering and ML implementation
- Real-world cybersecurity use case with web deployment

## License
- This project is for educational and demonstration purposes.
