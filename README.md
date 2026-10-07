# Multiple Disease Prediction System

A Streamlit-based machine learning web application that predicts the likelihood of common diseases using trained models and patient health parameters.

## Project Description

This project is designed to help users estimate disease risk based on medical input values. It includes:

- Diabetes prediction
- Heart disease prediction
- A placeholder section for Parkinson's disease prediction (not implemented yet)

The app uses machine learning models trained on publicly available datasets and allows users to enter values through a simple web interface.

## Features

- User-friendly dashboard built with Streamlit
- Multiple disease prediction options in a sidebar menu
- Diabetes model based on Logistic Regression
- Heart disease model based on Random Forest Classifier
- Model persistence using pickle files
- Scalable and easy-to-run local web application

## Tech Stack

- Python
- Streamlit
- Pandas
- NumPy
- scikit-learn
- Streamlit Option Menu

## Project Structure

```text
Multiple Disease Prediction/
├── project.py
├── requirements.txt
├── diabetes_model.sav
├── diabetes_scaler.sav
├── heart_model.sav
├── dataset/
│   ├── diabetes.csv
│   └── heart.csv
├── README.md
├── how to run.txt
├── TODO.md
└── PPT/
```

## Dataset

The project uses datasets stored in the `dataset` folder:

- `dataset/diabetes.csv`
- `dataset/heart.csv`

These files are used to train the diabetes and heart disease prediction models.

## Installation

1. Open a terminal in the project folder.
2. Install dependencies:

```bash
pip install -r requirements.txt
```

## Run the App

Start the Streamlit application with:

```bash
streamlit run project.py
```

## Usage

1. Open the web app in the browser.
2. Select a prediction type from the sidebar:
   - Diabetes Prediction
   - Heart Disease Prediction
3. Enter the required patient details.
4. Click the result button to see the predicted output and probability.

## Model Notes

- The diabetes model is saved as `diabetes_model.sav` and uses a scaler file `diabetes_scaler.sav`.
- The heart disease model is saved as `heart_model.sav`.
- If the model files do not exist, the app automatically trains them when run for the first time.
- Parkinson's disease prediction is currently marked as "not implemented yet".

## Important Note

This project is a beginner-friendly machine learning app for educational and demonstration purposes. It is not a substitute for professional medical diagnosis.

## License

This project is for learning and academic use.
