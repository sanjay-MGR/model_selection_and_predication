# MPG Prediction Project

A simple **Machine Learning** project that predicts **Miles Per Gallon (MPG)** of cars using the famous **Auto MPG** dataset.

---

## 📋 Project Overview

This project demonstrates the full machine learning workflow:
- Data exploration and preprocessing
- Training multiple regression models
- Model evaluation and selection
- Saving the best model
- Making batch predictions using the saved model

**Best Model:** `RandomForestRegressor`

---

## 📁 Project Files

| File | Description |
|------|-------------|
| `Model_selection_.ipynb` | Data loading, EDA, model training, evaluation, and saving the best model |
| `Predict_the_mpg_using_the_save_model_.ipynb` | Loading the saved model and predicting MPG on new data |
| `forest_model.pkl` | Trained Random Forest model (saved using joblib) |
| `input data to get the input.csv` | Input features used for prediction |
| `expanded_1000_rows.csv` | Expanded dataset (1000 rows) for batch prediction |
| `output_mpg.csv` | Predicted MPG values |
| `input with predicted .csv` | Combined input features + predictions |

---

## 🛠 Technologies Used

- **Python**
- **Pandas** & **NumPy** (Data handling)
- **Seaborn** & **Matplotlib** (Visualization)
- **Scikit-learn** (Modeling & Evaluation)
- **Joblib** (Model saving/loading)

---

## 📊 Dataset

- **Source**: Seaborn built-in `mpg` dataset
- **Target Variable**: `mpg` (Miles Per Gallon)
- **Features**:
  - cylinders
  - displacement
  - horsepower
  - weight
  - acceleration

---

## 🔍 Models Compared

| Model                    | Train R²     | Test R²      | Selected |
|-------------------------|--------------|--------------|----------|
| Linear Regression       | 0.699        | 0.727        | No       |
| Decision Tree           | 0.999        | 0.596        | No       |
| Support Vector Regressor| 0.684        | 0.745        | No       |
| **Random Forest**       | **0.965**    | **0.753**    | **Yes**  |

---

## 🚀 How to Use

### 1. Training the Model
Open `Model_selection_.ipynb` and run all cells. It will:
- Load and clean the data
- Train multiple models
- Save the best model as `forest_model.pkl`

### 2. Making Predictions
Open `Predict_the_mpg_using_the_save_model_.ipynb` and run all cells. It will:
- Load the saved model
- Predict MPG for new data
- Save predictions to CSV

---

## 📈 Results

- The **Random Forest Regressor** performed best with a **Test R² score of ~0.753**.
- Predictions for 1000 samples have been generated and saved.

---

## 🧩 Future Improvements

- Add more features (e.g., `model_year`, `origin`)
- Hyperparameter tuning
- Deploy as a web app (Streamlit/Gradio)
- Add data visualization dashboard

---

## 👤 Author

**Sanjaya**  
