## capstone-project: Predictive Maintenance Using NASA Turbofan Engine Dataset

# Project Overview

This capstone project investigates predictive maintenance using the NASA C-MAPSS Turbofan Engine Degradation Dataset.

The objective is to predict Remaining Useful Life (RUL) of aircraft engines using operational settings and sensor measurements.

# Research Question

Can machine learning models accurately predict the remaining useful life of an aircraft engine using historical sensor measurements?

# Dataset

NASA C-MAPSS Turbofan Engine Dataset

Training Dataset:
- 20,631 observations
- 26 original variables
- 100 engine units

Features include:
- Engine operational settings
- Sensor measurements
- Time cycles

# Data Cleaning

The dataset was evaluated for:

- Missing values
- Duplicate records
- Constant-value features

Results:
- No missing values
- No duplicate records
- Several low-information features identified

# Feature Engineering

Remaining Useful Life (RUL) was created using:

RUL = Maximum Engine Cycle − Current Cycle

This transformed the dataset into a supervised machine learning problem.

# Exploratory Data Analysis

Key findings:

- RUL distribution is right-skewed.
- Most engines fail between 170 and 230 cycles.
- Sensor_12, Sensor_7, Sensor_21, and Sensor_20 show strong positive relationships with RUL.
- Sensor_17, Sensor_15, Sensor_2, and Sensor_4 show strong negative relationships with RUL.

# Baseline Machine Learning Model

Model:
- Random Forest Regressor

Performance:

| Metric | Value |
|----------|----------|
| MAE | 25.45 |
| RMSE | 35.93 |
| R² | 0.7174 |

The model explains approximately 71.7% of the variation in Remaining Useful Life.

## Repository Structure
