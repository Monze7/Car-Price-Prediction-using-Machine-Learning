---

# 🚗 Car Price Prediction using Machine Learning

This project builds a regression model to predict **used car selling prices** based on features such as manufacturing year, kilometers driven, fuel type, transmission, and more.

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Google%20Colab-yellow?logo=googlecolab" />
  <img src="https://img.shields.io/badge/Machine%20Learning-Regression-blue" />
  <img src="https://img.shields.io/badge/Language-Python-orange" />
</p>

---

## 📁 Dataset

**Source:** [Kaggle - CarDekho Vehicle Dataset](https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho)

### Features:

* `name`: Name of the car
* `year`: Year of manufacture
* `selling_price`: Target variable (price to be predicted)
* `km_driven`: Total kilometers driven
* `fuel`: Type of fuel (Petrol, Diesel, etc.)
* `seller_type`: Who is selling the car
* `transmission`: Manual or automatic
* `owner`: Number of previous owners

---

## ⚙️ Workflow

### 1. Data Loading & Exploration

* Load CSV file into a DataFrame
* Explore dataset structure and check for missing values

### 2. Feature Engineering

* Create new feature: `car_age = current_year - year`

### 3. Preprocessing

* One-Hot Encoding for categorical features
* Scaling numeric features
* Train-test split

### 4. Model Building

Trained multiple regression models:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* Gradient Boosting Regressor

### 5. Evaluation

Used the following metrics:

* 📉 **Mean Squared Error (MSE)**
* 📈 **Root Mean Squared Error (RMSE)**
* 📊 **Mean Absolute Error (MAE)**
* 🧠 **R² Score**

---

## 📊 Results

| Model                       | R² Score |
| --------------------------- | -------- |
| Linear Regression           | 0.40     |
| Decision Tree Regressor     | 0.37     |
| Gradient Boosting Regressor | 0.48     |
| Random Forest Regressor     | 0.50     |

✅ **Best Model:** `Random Forest Regressor` (Explained \~50% of the variance in selling prices)

---

## ▶️ Run this on Google Colab

You can run the full notebook in Google Colab here:

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](YOUR_COLAB_NOTEBOOK_LINK_HERE)

---

## 🛠️ Setup Instructions

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/car-price-prediction.git
   cd car-price-prediction
   ```

2. Install the required libraries:

   ```bash
   pip install pandas numpy scikit-learn
   ```

3. Run the code in your local environment or open the notebook in Google Colab.

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repo and submit a PR.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

Let me know if you'd like a sample `requirements.txt`, Jupyter Notebook template, or the `Colab` version of the notebook with upload instructions!
