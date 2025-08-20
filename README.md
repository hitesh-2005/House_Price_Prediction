# House Price Prediction using Linear Regression

This project uses a simple **Linear Regression** model to predict house sale prices based on a few key features such as living area, number of bedrooms, and number of bathrooms. It provides basic data preprocessing, model training, evaluation, and visualization.

## 📂 Dataset

- **train.csv**: Contains training data with house features and actual `SalePrice`.
- **test.csv**: Contains test data for prediction (with or without actual `SalePrice`).

## 📌 Features Used

- `GrLivArea`: Above ground living area (in square feet)
- `BedroomAbvGr`: Number of bedrooms above ground
- `FullBath`: Number of full bathrooms
- `HalfBath`: Number of half bathrooms
- `TotalBath`: Derived feature = `FullBath + 0.5 * HalfBath`

## 🧠 Model

- **Model Used**: `LinearRegression` from `sklearn.linear_model`
- Features used for training: `GrLivArea`, `BedroomAbvGr`, `TotalBath`

## 📊 Evaluation Metrics

- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **R² Score**

These metrics are calculated on the training data and optionally on the test data if actual sale prices are available.

## 📈 Visualizations

1. **Actual vs Predicted Prices** scatter plot
2. Feature vs Price relationships:
   - `GrLivArea` vs `SalePrice`
   - `BedroomAbvGr` vs `SalePrice`
   - `TotalBath` vs `SalePrice`

## 📤 Predictions

- If `test.csv` does not contain `SalePrice`, predictions are saved in a file:
```

house\_price\_predictions.csv

````

## 📌 Feature Importance

Coefficients of the linear regression model are used to estimate the importance of each feature.

## 🛠 Requirements

Install required packages using pip:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
````

## ▶️ How to Run

1. Place `train.csv` and `test.csv` in the working directory.
2. Run the script:

   ```bash
   python house_price_prediction.py
   ```

## 📄 Output Files

* `house_price_predictions.csv`: Contains predicted house prices for test data (if target is not provided).

## 📬 Author

This project was created by Hitesh Gupta.

---

```


