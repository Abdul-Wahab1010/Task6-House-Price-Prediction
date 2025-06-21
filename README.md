# 🏠 Task 6: House Price Prediction

This project is part of my **AI/ML Engineering Internship** at **DevelopersHub Corporation**. It aims to build a predictive model to estimate house prices based on various property features. This task focuses on regression modeling, feature engineering, and model evaluation using real estate data.

---

## 🎯 Objective

To predict the price of a house using its features such as area (Marla), bedrooms, bathrooms, property type, city, and location.

---

## 📂 Dataset

- **File:** `house_data.csv`
- **Source:** [Kaggle Real Estate Dataset](https://www.kaggle.com/)
- **Records:** 3,000+ property listings
- **Features:**
  - `Area in Marla`, `bedroom`, `bathroom`, `Property_type`, `City`, `Location`, `purpose`
- **Target:** `Price` — Property price in PKR

---

## 🔧 Data Preprocessing

- Dropped irrelevant columns (`Serial#` if present)
- Filtered data for listings marked **"For Sale"**
- Encoded categorical features: `Property_type`, `City`, `Location`
- Applied `StandardScaler` for scaling numerical features
- Split into training and testing datasets (80/20 split)

---

## 📊 Exploratory Data Analysis (EDA)

- Analyzed feature distributions and outliers
- Plotted price trends with respect to area, bedrooms, and cities
- Visualized correlation matrix using heatmap
- Examined top factors affecting house price

---

## 🤖 Model Building

- **Algorithm:** `Linear Regression`
  - Simple and interpretable model for regression tasks
- Trained on scaled features
- Saved trained model as:
  - `house_price_model.pkl`  
  - `scaler.pkl` (for preprocessing future input)

---

## ✅ Evaluation Metrics

| Metric            | Result         |
|-------------------|----------------|
| Mean Absolute Error (MAE) | ~350,000 PKR |
| Root Mean Square Error (RMSE) | ~550,000 PKR |
| R² Score | ~0.78 |
| Visualization | 📈 Actual vs Predicted plot included |

---

## 💡 Key Insights

- **Area**, **Location**, and **City** have strong correlation with price.
- Encoding and proper scaling significantly improved model accuracy.
- The model generalizes well across test data and is useful for price estimations.

---

## 📁 Files Included

| File                             | Description                                 |
|----------------------------------|---------------------------------------------|
| `house_data.csv`                 | Cleaned dataset used for modeling           |
| `House_price_predication.ipynb` | Jupyter Notebook with full workflow         |
| `house_price_model.pkl`         | Trained Linear Regression model             |
| `scaler.pkl`                    | Scaler used during training                 |
| `README.md`                     | Project documentation                       |

---

## 🧠 Prediction Example

```python
new_house = pd.DataFrame([{
    'area_marla': 5,
    'bedroom': 3,
    'bathroom': 2,
    'property_type': 'House',
    'city': 'Lahore',
    'location': 'DHA Phase 5'
}])

 ```
## 💻 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/YourUsername/YourRepoName.git
cd YourRepoName

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

# 3. Run the notebook
jupyter notebook your_notebook_name.ipynb

```

## 📬 Author
Abdul Wahab
GitHub: @Abdul-Wahab1010
Internship Project – DevelopersHub Corporation | June 2025

