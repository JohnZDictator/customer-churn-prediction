# Churn Prediction Application

This project is a machine learning application built to predict customer churn for banks. It uses several machine learning models to analyze customer data and predict which customers are likely to churn, along with a web interface to display churn probabilities and generate personalized emails for each customer. 

---

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Demo](#demo)
- [Results](#results)
- [License](#license)

---

## Overview

This project leverages various machine learning models, such as XGBoost, Random Forest, Decision Trees, Naive Bayes, Logistic Regression, and Support Vector Classification, to predict customer churn. The web app provides a user-friendly interface displaying customer churn probabilities and generates a custom email for each customer using Llama3.

---

## Dataset

The application uses a dataset with customer information to train and test models. The data includes various customer attributes such as age, gender, tenure, product details, and account balance.

- **Source**: [Churn Dataset](churn.csv)

---

## Project Structure

```
├── data
│   └── churn.csv                     # Raw dataset file
├── models
│   └── xgboost_model.pkl             # Saved XGBoost model (and others)
├── notebooks
│   └── EDA.ipynb                     # Exploratory Data Analysis
├── app
│   ├── templates
│   │   └── index.html                # HTML for web interface
│   └── app.py                        # Flask app code
├── images
│   └── churn_probabilities.png       # Visualization images
├── README.md                         # This README file
└── requirements.txt                  # Python dependencies
```

---

## Technologies Used

- **Python**: Pandas, NumPy, Scikit-Learn, XGBoost
- **Machine Learning Models**: Random Forest, Decision Tree, XGBoost, Naive Bayes, Logistic Regression, Support Vector Classification
- **Flask**: For building the web application
- **Llama3**: To generate customized emails for customers based on churn predictions
- **Matplotlib**: For data visualization

---

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/churn-prediction-app.git
   cd churn-prediction-app
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Download or prepare the dataset**  
   Ensure the `churn.csv` file is in the `data` folder.

4. **Run the application**
   ```bash
   python app/app.py
   ```

---

## Usage

1. **Data Preparation**: Load and preprocess the dataset to handle missing values, split data, and visualize trends.
2. **Model Training**: Train various models and save the best-performing model (XGBoost) for the final application.
3. **Web App**: Open the app in a browser to view churn predictions and email summaries for customers.
4. **Email Generation**: Llama3 is used to generate personalized emails for each customer, explaining the churn analysis and offering solutions.

---

## Demo

### Example Predictions
![Churn Probabilities](images/churn_probabilities.png)

### Custom Email Generation
![Customer Email Example](images/customer_email_example.png)

---

## Results

The project successfully predicts customer churn and offers additional functionality:
- Improved recall on XGBoost model.
- Real-time churn predictions displayed on a web dashboard.
- Automated email generation explaining the results.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
