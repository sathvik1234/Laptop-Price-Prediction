Laptop Price Prediction

This project predicts laptop prices using machine learning models based on their specifications. The models are trained on historical laptop data including features like CPU, RAM, Storage, Screen Size, Weight, Touchscreen, GPU, and Operating System.

Project Overview

The goal of this project is to estimate the price of a laptop based on its features. It leverages multiple machine learning algorithms to achieve accurate predictions, including:

Random Forest Regressor

XGBoost Regressor

Gradient Boosting Regressor

Stacking Regressor (ensemble)

The dataset has been cleaned and preprocessed to handle missing values, convert categorical features using One-Hot Encoding, and calculate derived features such as PPI (Pixels Per Inch).

Dataset

The dataset includes the following features:

Feature	Description
Company	Laptop manufacturer (Apple, Dell, HP, etc.)
TypeName	Laptop type (Ultrabook, Notebook, Gaming, etc.)
Cpu	CPU model
Ram	RAM in GB
Memory	Storage type and size (SSD, HDD, Flash Storage)
Weight	Laptop weight in kg
TouchScreen	1 if laptop has touchscreen, else 0
Ips	1 if screen has IPS display, else 0
PPI	Pixels Per Inch (computed from resolution and screen size)
Cpu Name	Simplified CPU name
Cpu Brand	CPU brand
HDD	HDD storage in GB
SSD	SSD storage in GB
Gpu brand	GPU brand
os	Operating system
Price	Laptop price in INR

Additional derived features from Memory (HDD, SSD) and PPI are included for better model performance.

How to Use

Open the notebook
Open Laptop_Price_Prediction.ipynb in Google Colab or Jupyter Notebook.

Load the dataset and trained model

df.pkl : preprocessed dataset

pipe.pkl : trained pipeline for predicting prices

Run all cells step by step
This includes:

Data cleaning and preprocessing

Feature engineering (e.g., calculating PPI, splitting memory)

Training models (Random Forest, XGBoost, Stacking)

Evaluating models (R² score, MAE)
