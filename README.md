# 🌞 Solar Energy Generation Prediction

This project focuses on **predicting solar energy generation** using machine learning techniques, specifically **time-series forecasting** with the Prophet model.  
The dataset includes solar panel readings and environmental parameters that influence power generation.  
The notebook (`Solar_Energy_Generation.ipynb`) contains the full workflow: data preprocessing, visualization, model training, and evaluation, providing insights based on the predictions made and forecasting for December after training the model on data from January to November.

## ⚙️ Features

- Data preprocessing & cleaning  
- Exploratory Data Analysis (EDA) with visualizations  
- Time-series forecasting for solar energy prediction using **Prophet**  
- Evaluation of model performance using metrics like MAE, RMSE, R², and MAPE  
- Cross-location comparison and weather integration (NASA POWER daily data)  
- Easily extendable for real-world datasets  

## 🧠 Model Used

This project uses **Prophet** (from `facebook/prophet`) for forecasting solar power at each plant.  

**Why Prophet?**  
- **Time-series specialization:** Handles temporal patterns, ideal for 5-minute solar readings aggregated daily.  
- **Seasonality handling:** Models daily, weekly, and yearly seasonality, important for solar production.  
- **Robust to missing data & outliers:** Real-world sensor data often has gaps; Prophet manages these effectively.  
- **Flexible trend changepoints:** Locations 1 and 2 use `changepoint_prior_scale=0.08` to adapt to sudden changes without overfitting.  
- **Rapid prototyping:** Works directly with pandas DataFrames and requires minimal hyperparameter tuning.

**Workflow with the Model:**  
1. Preprocess and clean raw solar panel data.  
2. Aggregate 5-minute readings into daily energy output per plant.  
3. Merge with NASA POWER weather data (GHI, temperature, cloudiness, etc.).  
4. Train Prophet on historical data (November as training) and forecast December energy.  
5. Evaluate using MAE, RMSE, R², and MAPE.  

> Future work can replace or extend Prophet with more advanced models like **XGBoost**, **Neural Networks**, or **LSTM** for sequence modeling.

## Data

All datasets are organized under the `data/` folder:  

- `data/Location 1`  
- `data/Location 2`  
- `data/Location 3`  

## 🚀 Getting Started

### 1️⃣ Clone the repository

git clone https://github.com/Ashprogrammer29/Solar-Energy-Generation.git
cd Solar-Energy-Generation

### 2️⃣ Create and activate a virtual environment

python -m venv venv
venv\Scripts\activate   # On Windows
source venv/bin/activate   # On Mac/Linux

### 3️⃣ Install dependencies

pip install -r requirements.txt

### 4️⃣ Run the notebook

jupyter notebook Solar_Energy_Generation.ipynb

## 📦 Major Dependencies

Python 3.8+
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
prophet

### Install all dependencies with:

pip install -r requirements.txt

## 🛠️ Adding the data Folder to GitHub
Make a folder named data in your project:

mkdir data

## Copy your dataset into that folder. Example:

copy "C:\path\to\Location1" data\Location1
copy "C:\path\to\Location2" data\Location2
copy "C:\path\to\Location3" data\Location3

### Stage and commit the changes:

git add data/ 
git commit -m "Added dataset folder"
git push origin main

### ⚠️ If your dataset is large, consider using Git LFS or keep only a sample dataset in GitHub.

## 📌 Future Work
Add more advanced models (XGBoost, Neural Networks, LSTMs)
Deploy as a web application (Flask/Django/Streamlit)
Integrate real-time solar panel sensor data

### 👨‍💻 Author
Aswin Deiavanayagam
📧 Email: aswinsub9@gmail.com
📌 GitHub: Ashprogrammer29
