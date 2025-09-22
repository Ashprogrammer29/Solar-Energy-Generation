# 🌞 Solar Energy Generation Prediction

This project focuses on **predicting solar energy generation** using machine learning techniques.  
The dataset includes solar panel readings and environmental parameters that influence power generation.  
The notebook (`Solar_Energy_Generation.ipynb`) contains the full workflow: data preprocessing, visualization, model training, and evaluation.

## ⚙️ Features

- Data preprocessing & cleaning  
- Exploratory Data Analysis (EDA) with visualizations  
- Machine learning model training for solar energy prediction  
- Evaluation of model performance  
- Easily extendable for real-world datasets  

### Data

-Location 1
-Location 2
-Location 3


## 🚀 Getting Started

### 1️⃣ Clone the repository
git clone https://github.com/Ashprogrammer29/Solar-Energy-Generation.git
cd Solar-Energy-Generation


python -m venv venv
venv\Scripts\activate   # On Windows
source venv/bin/activate   # On Mac/Linux

##  Install dependencies

pip install -r requirements.txt

### Run the notebook

jupyter notebook Solar_Energy_Generation.ipynb



### 📦 Dependencies

List of major dependencies (full list in requirements.txt):

Python 3.8+
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter

### Install them with:

pip install -r requirements.txt


### 🛠️ Adding the data Folder to GitHub

Make a folder named data in your project:

mkdir data


Copy your dataset into that folder. Example:

copy "C:\path\to\solar_data.csv" data\


### Stage and commit the changes:

git add data/ 
git commit -m "Added dataset folder"
git push origin main


### ⚠️ If your dataset is large, consider using Git LFS or keep only a sample dataset in GitHub.


### 📌 Future Work

Add more advanced models (XGBoost, Neural Networks, LSTMs)
Deploy as a web application (Flask/Django/Streamlit)
Integrate real-time solar panel sensor data


### 👨‍💻 Author

Aswin Deiavanayagam

📧 Email: aswinsub9@gmail.com

📌 GitHub: Ashprogrammer29
