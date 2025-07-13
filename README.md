# 🚗 Vehicle Price Prediction using Machine Learning

## 📌 Objective
Predict vehicle prices based on key features like make, model, year, mileage, engine, fuel type, transmission, and body style using machine learning.

---

## 🛠️ Tools & Technologies Used

### 📚 **Programming & Libraries**
- **Python 3.12+**
- **pandas** (Data handling)
- **numpy** (Numerical operations)
- **matplotlib** (Visualizations)
- **seaborn** (Advanced visualizations)
- **scikit-learn** (Machine Learning Models & Pipeline)
- **joblib** (Model saving)


### ⚙️ **Machine Learning Techniques**
- Data Cleaning & Preprocessing
- Feature Engineering (Car Age)
- Encoding (OneHotEncoder)
- Scaling (StandardScaler)
- Model Training: RandomForestRegressor
- Model Evaluation: MAE, MSE, RMSE, R² Score


---

## 📂 Dataset Description
This dataset includes specifications and prices of vehicles.

| Column        | Description                       |
|---------------|-----------------------------------|
| make          | Manufacturer (e.g., Toyota, BMW)   |
| model         | Model name                         |
| fuel          | Fuel type (Gasoline, Diesel, etc.) |
| transmission  | Gear type (Automatic, Manual)      |
| trim          | Trim / Feature level               |
| body          | Body style (SUV, Sedan, etc.)      |
| exterior_color| Exterior paint color               |
| interior_color| Interior color                     |
| drivetrain    | AWD / FWD / RWD                    |
| engine        | Engine specification               |
| mileage       | Mileage in miles                   |
| cylinders     | Number of cylinders                |
| doors         | Number of doors                    |
| car_age       | Age of the vehicle in years         |
| price         | Price in USD (Target Variable)     |

---

## 🔍 Exploratory Data Analysis (EDA)
- Checked missing values
- Visualized correlations (mileage vs price, year vs price)
- Analyzed outliers in mileage & price columns

---

## 🧑‍💻 Machine Learning Pipeline

1️⃣ **Data Preprocessing**
- Handle missing values  
- Feature engineering (`car_age`)  
- Encode categorical features  
- Scale numerical features  

2️⃣ **Model Building**
- Train-Test Split (80/20)
- Random Forest Regressor (best performer)
- Pipeline (Preprocessor + Model)

3️⃣ **Evaluation Metrics**
| Metric   | Interpretation               |
|----------|-------------------------------|
| MAE      | Mean Absolute Error (lower = better) |
| MSE      | Mean Squared Error            |
| RMSE     | Root Mean Squared Error        |
| R² Score | Variance explained by model (closer to 1 is better) |

---

---

## 🚀 Running the Project Locally

### 1️⃣ Clone Repository
```bash
git clone https://github.com/yourusername/vehicle-price-prediction.git
cd vehicle-price-prediction
```

pip install -r requirements.txt

## 📝 Sample Model Performance (Results)
## 📊 Model Evaluation Results

| Metric                          | Value           |
|---------------------------------|-----------------|
| **Mean Absolute Error (MAE)**   | **4,670.57 USD**   |
| **Mean Squared Error (MSE)**    | **67,689,853.03 USD²** |
| **Root Mean Squared Error (RMSE)** | **8,227.38 USD**   |
| **R² Score**                    | **0.7783**         |

---

### 🔍 Interpretation:
- **MAE ~ 4670 USD**: On average, predictions deviate by about **$4670** from actual prices.
- **RMSE ~ 8227 USD**: Larger errors are present but within an acceptable range for vehicle price prediction.
- **R² ~ 0.7783**: The model explains approximately **77.8% of the variance** in vehicle prices, showing solid performance.

