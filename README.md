Here’s a detailed README file for your project, explaining how to access and use it:

---

# NYC Airbnb Market Analysis

This project provides insights into the New York City Airbnb market, focusing on pricing trends, occupancy rates, and other significant factors. The analysis includes data preprocessing, feature engineering, model training, and evaluation using Gradient Boosting.

## Features

* **Data Cleaning:** Handling missing and infinite values.
* **Feature Engineering:** Transformations for better predictive capabilities.
* **Model Training:** Gradient Boosting Regressor for price prediction.
* **Evaluation Metrics:** MAE and R² score to evaluate model performance.
* **Reusable Model:** Exported trained model for future predictions.

---

## File Structure

```
NYC_Airbnb_Market_Analysis/
│
├── listings.csv                # Original dataset
├── nyc_airbnb_analytics.ipynb  # Jupyter Notebook with code and analysis
├── gradient_boosting_model.pkl # Trained Gradient Boosting model
├── README.md                   # Project overview and usage guide
```

---

## Getting Started

### Prerequisites

* Python 3.8+
* Jupyter Notebook
* Required Python libraries: `pandas`, `numpy`, `scikit-learn`, `joblib`, `matplotlib`

Install dependencies using:

```bash
pip install -r requirements.txt
```

### Accessing the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/Geetvardhan/NYC-Airbnb-Market-Analysis.git
   ```

2. Navigate to the project directory:

   ```bash
   cd NYC-Airbnb-Market-Analysis
   ```

3. Open the Jupyter Notebook:

   ```bash
   jupyter notebook nyc_airbnb_analytics.ipynb
   ```

---

## How to Use the Trained Model

1. Load the `gradient_boosting_model.pkl` file:

   ```python
   import joblib
   model = joblib.load("gradient_boosting_model.pkl")
   ```

2. Make predictions:

   ```python
   sample_data = [[1, 40.7128, -74.0060, 3, 5, 0.3, 1, 365, 1, 5000, 2, 1, 0.05]]
   prediction = model.predict(sample_data)
   print("Predicted Price:", prediction)
   ```

---

## Results

* **MAE:** 1.49
* **R² Score:** 0.965

These metrics indicate a highly accurate model capable of making reliable predictions.

---

## Contributions

Feel free to open issues or submit pull requests to enhance this project!

---

Let me know if you'd like any modifications!
