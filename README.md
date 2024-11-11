# Employee Retention Analytics Platform

An end-to-end predictive analytics platform that uses machine learning to forecast employee attrition and provides actionable insights for HR professionals to improve retention strategies.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Tech Stack](#tech-stack)
4. [Machine Learning Workflow](#machine-learning-workflow)
5. [Setup and Installation](#setup-and-installation)
6. [Usage](#usage)
---

## Project Overview

The **Employee Retention Analytics Platform** is designed to help organizations understand and reduce employee attrition. The platform combines data processing, machine learning, and a full-stack web interface to provide HR departments with actionable insights into key factors that affect employee retention, helping them take proactive steps to retain valuable team members.

This project was built using a full-stack approach with a **Spring Boot** backend and **React** frontend, and it integrates a **machine learning model** trained on employee data to predict attrition likelihood.

## Features

- **Attrition Prediction**: Predicts the likelihood of an employee leaving the organization based on personal and organizational factors.
- **Interactive Data Visualizations**: Displays insights such as job satisfaction, work-life balance scores, and trends in employee exits.
- **Employee Profiles**: View detailed profiles with a breakdown of attrition risk factors.
- **Filter & Analyze**: Analyze attrition risk based on job roles, departments, tenure, and other factors.
- **Secure Data Management**: Role-based access control with JWT authentication to ensure data security.

## Tech Stack

- **Frontend**: React, Tailwind CSS, Chart.js for visualizations
- **Backend**: Spring Boot, Spring Security (JWT for authentication)
- **Database**: MySql
- **Machine Learning**: Python, Scikit-Learn, SHAP for interpretability
- **Deployment**: Docker, AWS (or Heroku)

## Machine Learning Workflow

1. **Data Collection & Preprocessing**  
   The dataset contains employee data such as age, job role, job satisfaction, work-life balance, and exit status. We handled missing values, performed one-hot encoding for categorical variables, and normalized numerical features to prepare the data.

2. **Feature Engineering**  
   Key features impacting employee attrition were selected based on domain knowledge and exploratory data analysis (EDA). Features such as work-life balance, job satisfaction, and distance from home were retained for model training.

3. **Model Selection & Tuning**  
   Several classification models were evaluated, including Logistic Regression, Decision Trees, and Random Forest. Hyperparameter tuning was conducted to improve the F1 score, which is essential in handling imbalanced datasets (as retention typically shows class imbalance).

4. **Explainability with SHAP**  
   SHAP (SHapley Additive exPlanations) values were used to interpret feature importance, helping HR professionals understand what factors influence an employee’s risk of leaving.

5. **Model Deployment**  
   The final model was integrated into the Spring Boot backend as a REST API endpoint, allowing real-time predictions and batch processing.

## Setup and Installation

### Prerequisites

- [Node.js](https://nodejs.org/)
- [Java 11+](https://www.oracle.com/java/technologies/javase-downloads.html)
- [MySQL](https://www.mysql.com/)
- [Python 3.x](https://www.python.org/)

### Backend Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/employee-retention-platform.git
   cd employee-retention-platform
### Usage
1. Login to the platform with an HR account.
2. Access the Employee Dashboard to see predictions and insights on retention.
3. Explore individual employee profiles and predict exit status in real-time.
4. Use interactive charts to analyze factors impacting attrition across the organization.
