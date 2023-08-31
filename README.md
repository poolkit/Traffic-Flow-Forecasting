# Multivariate Road Traffic Forecasting
![](/images/traffic.jpg)
## Overview

This project utilizes multivariate time series forecasting with LSTM (Long Short-Term Memory) to predict road traffic conditions. The data for this project was fetched from the UK National Highway website through their API and supplemented with weather data from a separate API. The project is implemented using Python and Jupyter Notebook.

## Table of Contents

- [Project Structure](#project-structure)
- [Data Collection](#data-collection)
- [Data Preprocessing](#data-preprocessing)
- [Model Training](#model-training)
- [Model Evaluation](#model-evaluation)
- [Results](#results)
- [Conclusion](#conclusion)

## Project Structure

The project is organized as follows:

- `dataset/`: Contains the fetched/processed traffic and weather data.
- `notebooks/`: Jupyter notebooks for data preprocessing, model training, and evaluation.
- `saved/`: Saved model checkpoints and pickle objects.
- `requirements.txt`
- `README.md`: This README file.

## Data Collection

Data for this project was collected from two sources:

- [UK National Highway API](https://webtris.highwaysengland.co.uk/api/swagger/ui/index): This API fetched road traffic data for the desired dates.
- [Weather API](https://open-meteo.com/en/docs/historical-weather-api): Weather data was obtained from a separate API for the exact dates.
- Instructions for data retrieval can be found in the data collection notebook (notebooks/FetchData.ipynb).

## Data Preprocessing

Data preprocessing is a crucial step in preparing the data for training. This includes EDA, data cleaning, feature engineering, and handling missing values. Detailed preprocessing steps are documented in the notebooks/Preprocessing.ipynb notebook.

## Model Training
The core of this project is the LSTM-based multivariate time series forecasting model. The model training process can be found in the notebooks/Training.ipynb notebook. You can adjust hyperparameters, model architecture, and other settings as needed for your specific use case.

## Model Evaluation
To assess the model's performance and how it performs on future data, MSE and visualizations are provided in the notebooks/Testing.ipynb notebook.

## Results
After training and evaluating the model, I achieved promising results in predicting road traffic conditions for 2 days in advance. The Mean Squared Error (MSE) on unseen data was measured at 3682.81, demonstrating the model's ability to provide accurate predictions.

## Conclusion
In this project, we successfully implemented a multivariate time series forecasting model using LSTM to predict road traffic conditions based on data from the UK National Highway and weather information. The project demonstrates the potential for accurate traffic forecasting, which can have practical applications in traffic management and planning.
