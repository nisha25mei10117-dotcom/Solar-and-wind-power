# Solar-and-wind-power
DATASETS for solar-and-wind-power
PROJECT TITLE: 
Solar-and-wind-power-generations.
OVERVIEW: 
This repository contains a curated dataset focused on solar and wind power generation. it includes historical measurements of energy production, weather parameters, and turbine/solar perfomance indicators. The dataset is ideal for machine learning, renewable energy forecasting, time-series analysis, and reasearch on sustainable energy systems.
FEATURES:
Multi-source renewable energy data (solar panels + wind turbines)
Time-series format (hourly/daily records)
Weather variables such as:
Solar irradiance
Temperature
Wind speed & direction
Humidity
Atmospheric pressure
Cleaned & structured CSV files
Ready for:
Forecasting models
Load balancing simulations
Energy optimization algorithms
Includes metadata for easy understanding of each column.
INSTALLATION:
1. Clone the Repository
git clone https://github.com/your-username/solar-wind-dataset.git
cd solar-wind-dataset
2. Set Up Environment (optional)
If you want to run analysis scripts:
python -m venv venv
source venv/bin/activate       # Linux/Mac
venv\Scripts\activate          # Windows
3. Install Dependencies
pip install -r requirements.txt
TESTING AND USAGE:
1. Load the Dataset
import pandas as pd
df = pd.read_csv('data/solar_wind_generation.csv')
print(df.head())
2. Basic Statistics
df.describe()
3. Plot Power Generation (optional)
import matplotlib.pyplot as plt
plt.figure(figsize=(10,5))
plt.plot(df['timestamp'], df['solar_power'], label='Solar')
plt.plot(df['timestamp'], df['wind_power'], label='Wind')
plt.legend()
plt.xlabel("Time")
plt.ylabel("Power (kW)")
plt.title("Solar & Wind Power Generation Over Time")
plt.show()
4. Run the Test Script (if included)
python test_dataset.py
