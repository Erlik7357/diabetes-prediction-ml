# Diabetes Prediction ML

Classification of diabetic and non-diabetic patients using a Support Vector Machine (SVM) algorithm.

## Overview

This project uses a Support Vector Machine classifier trained on health-related input features to predict whether a person is diabetic or non-diabetic. The trained model and the corresponding data scaler are saved and reused for making predictions on new input data.

## Project Structure

```
diabetes-prediction-ml/
├── diabetes.csv
├── diabetes_prediction.py
├── model.pkl
├── scaler.pkl
├── requirements.txt
└── README.md
```

| File | Description |
|---|---|
| `diabetes.csv` | Dataset used for training and testing the model |
| `diabetes_prediction.py` | Main script for training/loading the model and running predictions |
| `model.pkl` | Serialized (pre-trained) SVM model |
| `scaler.pkl` | Serialized scaler used to normalize input features |
| `requirements.txt` | List of required Python packages |
| `README.md` | Project documentation |

## Requirements

- Python 3.7 or higher
- numpy
- pandas
- scikit-learn

## Installation

Install all required libraries using the requirements file:

```bash
pip install -r requirements.txt
```

Or install the dependencies manually:

```bash
pip install numpy pandas scikit-learn
```

## Usage

Run the prediction script from the terminal:

```bash
python diabetes_prediction.py
```

When prompted, enter the required input values (e.g., glucose level, blood pressure, BMI, age, etc., as defined in `diabetes.csv`). The script will load the pre-trained model and scaler, process the input, and display whether the prediction is diabetic or non-diabetic.

## How It Works

1. The dataset (`diabetes.csv`) is loaded and preprocessed.
2. Input features are normalized using the saved scaler (`scaler.pkl`).
3. The trained SVM model (`model.pkl`) takes the scaled input and outputs a classification: diabetic or non-diabetic.
4. The result is displayed to the user in the terminal.

## Getting Help

If you face any issues while using this project:

- Open an issue in this repository.
- Contact the maintainer directly.
- Review the documentation and inline comments within the code.

## Maintainer

**Lalit Karela**
Agri-Entrepreneur

## License

This project is maintained and developed for educational and practical learning purposes.
