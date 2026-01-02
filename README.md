# energy-consumption-prediction
Machine learning project forecasting household energy usage with TensorFlow and Keras.

# Appliance Energy Consumption Prediction
This project uses a **deep learning model (TensorFlow/Keras)** to predict household appliance energy consumption based on environmental features such as temperature, humidity, wind speed, visibility, and pressure.  

The dataset used is **[Energy Data Complete](https://archive.ics.uci.edu/ml/datasets/Appliances+energy+prediction)**, which contains detailed records of indoor and outdoor conditions along with appliance energy usage.

---

# Project Structure
- `energy_prediction.py` → Main script with data preprocessing, model training, evaluation, and visualization.
- `energydata_complete.csv` → Dataset (if included, otherwise provide download link).
- `README.md` → Project documentation.

---

# Features
- **Data Preprocessing**: Standardization using `StandardScaler`.
- **Model Architecture**: Multi-layer neural network with ReLU activations.
- **Evaluation Metrics**: Mean Squared Error (MSE) and R² Score.
- **Visualizations**:
  - Actual vs Predicted appliance energy consumption.
  - Training vs Validation loss curves.
- **Sample Prediction Report**: Generates a tabular report for custom input values.

---

#  How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/rahulchandra2004/appliance-energy-prediction.git
   cd appliance-energy-prediction
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   *(Create a `requirements.txt` with packages like `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `tensorflow`.)*
3. Run the script:
   ```bash
   python Rahul_Energy_Consumption_prediction.py
   ```

---

# Sample Output
```
=== Energy Consumption Prediction Report ===

 Temperature (°C)  Humidity (%)  Wind Speed (km/h)  Visibility (km)  Pressure (mmHg)  Predicted Energy Consumption (Wh)
              20            40                  3               40              760                             45.67
```

---

# Future Improvements
- Add **LSTM/GRU models** for time-series forecasting.
- Hyperparameter tuning with **Keras Tuner**.
- Deploy as a **web app** using Flask/Django + React.
- Integrate **live IoT sensor data** for real-time predictions.


---

# Acknowledgements
- Dataset: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Appliances+energy+prediction)
- Libraries: TensorFlow, Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn
```
