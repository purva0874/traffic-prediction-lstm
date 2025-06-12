# Traffic Volume Prediction using LSTM

This project uses a Long Short-Term Memory (LSTM) neural network to forecast hourly vehicle traffic at a city road junction based on historical time series data.

## Problem Statement : Forecast hourly vehicle count using the past 24 hours of traffic data from a road junction to assist in urban traffic planning and congestion management.

---

## Dataset
- **Source**: Real-world dataset collected hourly from traffic junctions.
- **Columns used**:  
  - `DateTime` – timestamp of the record  
  - `Junction` – road junction ID (filtered for Junction 1)  
  - `Vehicles` – number of vehicles counted in that hour

---

## ML Approach
- Supervised learning using **LSTM neural network**
- Model input: Previous 24-hour traffic data
- Model output: Predicted vehicle count for the next hour

---

## Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-learn  
- TensorFlow / Keras  
- Matplotlib

---

## Model Summary
- Scaled data using `MinMaxScaler`
- Created sequences of length 24 (one day)
- Trained LSTM model with one LSTM layer and one Dense output layer

---

## Results
- **Mean Absolute Error (MAE)**: ~4.57 vehicles/hour  
- **Mean Squared Error (MSE)**: ~40.83  
- Plotted predicted vs actual traffic volume for evaluation

---

## Example Output
```python
Predicted traffic for next hour: 70.48 vehicles
