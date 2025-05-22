# CNC-Cost-Estimation


## 🔍 Overview
This project aims to build a simple machine learning model to estimate the CNC machining cost of a part using features such as material, dimensions, and derived metrics like volume and surface area.

---

## 📁 Dataset
- Manually created dataset with columns:
  - Material
  - Length, Width, Height
  - Quoted_Cost
  - Volume (engineered)
  - Cost_per_mm³ (engineered)
  - Surface Area (engineered)
  - SA/Volume Ratio (engineered)

---

## 🧼 Data Preprocessing
- Cleaned column headers
- Removed or handled missing data
- Converted categorical data using One-Hot Encoding

---

## ⚙️ Feature Engineering
- Volume = Length × Width × Height
- Surface Area = 2 × (L×W + W×H + H×L)
- Cost_per_mm³ = Quoted_Cost / Volume
- SA/Volume Ratio = Surface_Area / Volume

---

## 📊 Visualizations & Modeling
- Correlation heatmaps
- Material-wise cost trends
- Trained a Linear Regression model
- Evaluation metrics:
  - MAE, RMSE
  - Feature importance (coefficients)

---

## ✅ Results
- Height, Volume, and Material_Titanium showed strong influence on cost
- Linear model worked decently for small dataset
- RMSE and MAE calculated (included in the notebook)

---

## 💡 Reflection
- More real-world data would improve model accuracy
- Tool complexity, feature count, tolerance could be useful future features

---

## 📁 Files
- `CNC_Cost_Estimation.ipynb` – Jupyter Notebook
- `README.md` – Project summary
- `dataset.csv` – (If submitted)

---


