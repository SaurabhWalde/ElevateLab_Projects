# Customer Lifetime Value (LTV) Prediction

This project predicts the **Customer Lifetime Value (LTV)** using historical purchase behavior, allowing for **targeted marketing** and **customer segmentation**.

---

## 📁 Folder Structure

```

project1_clv/
├── ltv_prediction.ipynb           # Jupyter Notebook with full workflow
├── customer_data.csv              # Raw transactional customer data
├── customer_ltv_predictions.csv   # Final LTV predictions with segments
├── ltv_xgb_model.pkl              # Trained XGBoost model
├── power_transformer.pkl          # PowerTransformer for target scaling
├── scaler.pkl                     # StandardScaler for feature normalization
├── report.pdf                     # Two-page summary report
├── README.md 
├── requirements.txt 
````

---

## 🔍 Objective

Predict LTV from purchase data using engineered features such as:

- **Recency** – Days since last purchase
- **Frequency** – Number of unique purchases
- **AOV** – Average Order Value
- **Product Variety**, **Purchase Interval**

---

## 🛠 Tools Used

- Python (Pandas, Sklearn, XGBoost)
- Matplotlib & Seaborn for visualization
- Jupyter Notebook
- Excel for quick inspection

---

## 🧠 ML Model

- Model: **XGBoost Regressor**
- Target: Log-transformed `Monetary` (total spend)
- Evaluation:
  - MAE
  - RMSE
  - R²
- Customer segmentation using predicted LTV (Low / Medium / High)

---

## 📊 Visualizations

15 charts included:
- Monetary, Recency, Frequency Distributions
- Monthly Sales Trends
- Feature Correlations
- Customer Segmentation KDE
- Country-wise Distribution & more

---

## 📦 Outputs

- Trained model: `ltv_xgb_model.pkl`
- Scaler: `scaler.pkl`
- Transformer: `power_transformer.pkl`
- Final prediction CSV: `customer_ltv_predictions.csv`

---

## 📑 Report

Detailed 2-page analysis of the approach and results in `report.pdf`.

---

## 📌 Usage

To re-run:

```python
# Inside a Jupyter Notebook or Python script
!pip install -r requirements.txt

# Then run:
python ltv_prediction.ipynb
````

---
