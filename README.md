# MAI5043-House-Price-Prediction
House price prediction using Linear Regression and optimized Random Forest Regression.
# House Price Prediction Using Machine Learning

## Project Overview

This project was developed for MAI5043 Applied Machine Learning. It applies supervised machine learning techniques to predict residential property sale prices using the Kaggle House Prices – Advanced Regression Techniques dataset.

## Dataset

The project uses the Ames Housing dataset, which contains 1,460 labelled training observations and 1,459 unlabelled Kaggle test observations.

Dataset source: https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data

## Methodology

The machine learning workflow consists of:

1. Exploratory Data Analysis (EDA)
2. Missing-value handling and preprocessing
3. Feature engineering and categorical encoding
4. Linear Regression and Random Forest Regression
5. Model training and evaluation
6. Hyperparameter tuning using GridSearchCV
7. Model comparison and prediction-error analysis

## Model Performance

| Model | MAE (USD) | RMSE (USD) | R² |
|---|---:|---:|---:|
| Linear Regression | 20,692.57 | 31,611.52 | 0.8697 |
| Original Random Forest | 17,433.97 | 29,418.52 | 0.8872 |
| Optimized Random Forest | 17,224.73 | 29,216.76 | 0.8887 |

The optimized Random Forest achieved a 0.69% reduction in held-out RMSE compared with the original model.

## Technologies Used

- Python
- Google Colab
- pandas and NumPy
- scikit-learn
- Matplotlib and Seaborn

## How to Run

1. Download `train.csv` and `test.csv` from the Kaggle dataset page.
2. Open the `.ipynb` notebook in Google Colab.
3. Upload both dataset files to the Colab `/content` directory.
4. Run the notebook cells in order.
5. Find the generated graphs and CSV result files in the `MAI5043_Results` directory.

## Project Structure

- Notebook: Executable Python implementation
- `results/`: Saved evaluation metrics, tuning results and predictions
- `figures/`: Generated EDA and model evaluation visualizations

## Key Findings

Random Forest Regression outperformed Linear Regression on the held-out evaluation set. Hyperparameter tuning produced a small improvement in predictive accuracy, although prediction errors remained higher for some expensive properties.
