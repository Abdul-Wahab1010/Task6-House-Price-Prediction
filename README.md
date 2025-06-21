# 🏠 Task 6: House Price Prediction

This project aims to build a regression model to predict house prices based on property features such as area, bedrooms, bathrooms, city, and location.

## 📊 Dataset

- **Name:** House Price Prediction Dataset
- **Source:** [Kaggle](https://www.kaggle.com/)
- **Shape:** ~2000 rows, 9 columns
- **Key Features:**
  - `area_marla`: Size of the house in Marla
  - `bedroom`: Number of bedrooms
  - `bathroom`: Number of bathrooms
  - `property_type`: Type of property (House, Flat, etc.)
  - `city`: City name
  - `location`: Specific location within the city
  - `price`: (Target) Price of the property

## ⚙️ Preprocessing Steps

- Filtered only listings with `purpose = For Sale`
- Removed irrelevant columns like `Serial#`
- Handled categorical features using Label Encoding for model training
- Split data into training and test sets

## 🤖 Models Used

- **Linear Regression**

## 📈 Evaluation Metrics

- **Mean Absolute Error (MAE):** Measures average absolute prediction error
- **Root Mean Squared Error (RMSE):** Penalizes large errors

MAE: 4,90,000 PKR
RMSE: 7,30,000 PKR


## 📉 Visualization

- Correlation Heatmap
- Actual vs. Predicted Price Scatter Plot

## 💡 Insights

- House area (`area_marla`), number of bedrooms and bathrooms strongly influence house price.
- City and specific location also significantly affect property value.

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

