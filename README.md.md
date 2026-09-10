# Car Price Prediction

This project is a reproducible Jupyter Notebook for the OASIS INFOBYTE Data Science Task 3.

## Run it

1. Create and activate a Python environment.
2. Install dependencies: `pip install -r requirements.txt`
3. Start Jupyter with `jupyter notebook` and run `car_price_prediction.ipynb` from top to bottom.

`car_data.csv` is included beside the notebook. The supplied source contains a mix of cars and two-wheelers; the notebook explicitly removes two-wheeler records before building the car-only model.

## Verified run summary

The supplied 301-row file yielded 200 car records after removing 2 duplicates and 99 two-wheelers. On a fixed 80/20 split (`random_state=42`), Random Forest was the best model: MAE 0.976 lakh INR, RMSE 1.479 lakh INR, and R² 0.873.

## Scope and caution

Selling prices and `Present_Price` are measured in Indian lakh rupees. This is an educational regression exercise, not a valuation tool; performance can vary substantially outside the dataset's market, model years, and vehicle mix.
