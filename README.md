# California Housing Price Prediction

This repository contains an end-to-end **regression analysis** on the **California Housing Dataset**. The project includes **data cleaning, exploratory data analysis (EDA), feature scaling, and regression modeling** using five different algorithms.

## Project Overview

The goal of this project is to predict **median house values** in California based on various housing-related features. The dataset includes information such as **longitude, latitude, housing age, total rooms, total bedrooms, population, households, median income, and ocean proximity**.

## Dataset

The dataset used is **Cali-price.csv**, which contains **20,640** records with **10 columns**.

## Workflow

1. **Data Cleaning:**
   - Filled missing values in `total_bedrooms` using the median.
   - Encoded categorical variable `ocean_proximity` using one-hot encoding.

2. **Exploratory Data Analysis (EDA):**
   - Generated a correlation heatmap to understand feature relationships.
   - Visualized the distribution of house prices.
   - Explored the relationship between **median income and house prices**.

3. **Feature Scaling:**
   - Applied **StandardScaler** to numerical features to standardize data before training.

4. **Regression Models Used:**
   - **Linear Regression**
   - **Ridge Regression**
   - **Random Forest Regressor**
   - **Gradient Boosting Regressor**
   - **Support Vector Regressor (SVR)**

5. **Model Evaluation:**
   - Evaluated performance using **Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² Score**.
   
## Results

| Model                     | MAE        | RMSE       | R² Score  |
|---------------------------|------------|------------|------------|
| Linear Regression         | 50,670.74  | 70,060.52  | 0.6254     |
| Ridge Regression          | 50,678.36  | 70,068.81  | 0.6253     |
| Random Forest Regressor   | 31,631.02  | 49,008.79  | 0.8167     |
| Gradient Boosting Regressor | 38,248.74  | 55,888.27  | 0.7616     |
| Support Vector Regressor  | 87,055.05  | 116,925.19 | -0.0433    |

- **Random Forest Regressor performed the best** with the highest R² Score (0.8167) and lowest errors.
- **Support Vector Regressor (SVR) performed the worst**, likely due to poor kernel choice or hyperparameter tuning needs.

## How to Run

1. Clone the repository:
   ```sh
   git clone https://github.com/your_username/california-housing-prediction.git
   cd california-housing-prediction
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the script:
   ```sh
   python housing_price_prediction.py
   ```

## Requirements
Ensure you have the following Python libraries installed:
```sh
numpy
pandas
matplotlib
seaborn
scikit-learn
```
## Author
[John Ray Tran]


