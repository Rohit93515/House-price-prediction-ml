# House Price Prediction System

An end-to-end Machine Learning project that estimates residential
property prices using property characteristics and location features.

## Features

- Exploratory Data Analysis (EDA)
- Missing-value and duplicate checks
- City-wise price analysis
- Correlation analysis
- Linear Regression baseline
- Random Forest Regression
- Hyperparameter tuning with cross-validation
- Actual vs. predicted price visualization
- Interactive Gradio web application
- Prediction history and CSV export
- Model evaluation dashboard

## Dataset

- Records: 80,000
- Features: 18 columns, including the target
- Target: `Price_INR_Lakhs`
- Dataset type: Synthetic

Features include city, locality type, property type, BHK, bathrooms,
super area, carpet area, furnishing, parking, lift, and distances.

## Model Performance

| Metric | Tuned Random Forest |
|---|---:|
| MAE | 32.90 lakhs |
| RMSE | 68.92 lakhs |
| R² Score | 0.7855 |

Metrics are from the reported held-out test evaluation.
Results may vary with the dataset split and model version.

## Tech Stack

- Python
- Pandas and NumPy
- Matplotlib
- Scikit-learn
- Gradio
- Joblib
- Google Colab

## Run the Project

1. Open the notebook in Google Colab.
2. Install the required Python libraries.
3. Load the trained model or run the training notebook.
4. Launch the Gradio application.
5. Enter property details and view the estimated price.

## Limitations

This project uses a synthetic dataset. Predictions demonstrate
a machine-learning workflow and are not verified real-estate
market valuations. MAE and RMSE indicate meaningful prediction
errors, especially for some high-value properties.

## Future Improvements

- Validate on a real-world property dataset
- Improve performance on high-price properties
- Add explainability using SHAP
- Add persistent prediction storage
- Deploy the app using a hosted application platform
