🦠 Disease Spread Modeling and Simulation with Machine Learning
📌 Overview

This project focuses on modeling and simulating disease spread using Agent-Based Modeling (ABM) and applying Machine Learning regression models to predict the peak number of infected individuals based on simulation parameters.
The simulation is implemented using the Mesa framework, and multiple ML models are evaluated to determine which model best predicts disease spread outcomes.

This project combines:

Agent-Based Modeling

Simulation Data Generation

Machine Learning Regression

Model Performance Comparison

Data Visualization

🎯 Objectives

Simulate disease spread in a population using Agent-Based Modeling

Generate synthetic simulation datasets

Predict peak infection count using Machine Learning

Compare performance of multiple regression models

Visualize and analyze model performance

🧠 Modeling Approach
Agent-Based Model (Mesa Framework)

Each individual in the population is represented as an agent with one of the following states:

S (Susceptible) – Healthy, can get infected

I (Infected) – Currently infected

R (Recovered) – Recovered from infection

Agents interact and change states based on:

Infection rate

Recovery rate

Population size

Initial infected individuals

Simulation steps

⚙️ Simulation Parameters
Parameter	Description
population	Total number of individuals
infection_rate	Probability of infection
recovery_rate	Probability of recovery
initial_infected	Number of initially infected individuals
steps	Simulation duration
📊 Dataset Generation

The simulation is run 1000 times with randomized parameters to generate a dataset.

Generated file:

simulation_data.csv


Columns:

population

infection_rate

recovery_rate

initial_infected

steps

peak_infected (target variable)

🤖 Machine Learning Models Used

The following regression models were trained and evaluated:

Linear Regression

Decision Tree Regressor

Random Forest Regressor

Gradient Boosting Regressor

Support Vector Regressor (SVR)

K-Nearest Neighbors Regressor

📈 Evaluation Metrics

Models were evaluated using:

R² Score

RMSE (Root Mean Squared Error)

MAE (Mean Absolute Error)

Generated file:

model_comparison.csv

📉 Visualizations

The project generates performance comparison graphs:

model_r2_comparison.png

model_rmse_comparison.png

These help identify the best performing ML model.

🛠️ Technologies Used

Python

Mesa (Agent-Based Modeling)

NumPy

Pandas

Scikit-learn

Matplotlib

📂 Project Structure
Modelling_and_Simulation.ipynb
simulation_data.csv
model_comparison.csv
model_r2_comparison.png
model_rmse_comparison.png
README.md
