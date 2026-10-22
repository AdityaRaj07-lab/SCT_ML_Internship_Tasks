# SCT_ML_Internship_Tasks

Machine Learning internship tasks for **SkillCraft Technology**. Each task is a self-contained Google Colab notebook (Python, pandas, NumPy, scikit-learn, Matplotlib).

| # | Task | Algorithm | Notebook | Status |
|---|------|-----------|----------|--------|
| 1 | House Price Prediction | Linear Regression | `SCT_ML_Task1_House_Price_Prediction.ipynb` | Done |
| 2 | Mall Customer Segmentation | K-Means | `SCT_ML_Task2_Customer_Segmentation.ipynb` | Done |
| 3 | Cat vs Dog Classification | SVM | `SCT_ML_Task3_Cat_Dog_SVM.ipynb` | In progress |
| 4 | Hand Gesture Recognition | TBD | `SCT_ML_Task4_Hand_Gesture_Recognition.ipynb` | In progress |

## Task 1 — House Price Prediction
- **Goal:** predict sale price from square footage, bedrooms and bathrooms.
- **Dataset:** Ames Housing (`train.csv` from Kaggle's *House Prices: Advanced Regression Techniques*), 1,460 rows. Columns used: `GrLivArea`, `BedroomAbvGr`, `FullBath`+0.5×`HalfBath`, `SalePrice`.
- **Method:** cleaning (invalid records, houses > 4,000 sq ft removed), 80/20 split, `LinearRegression`.
- **Metrics:** MAE, RMSE, R² on the held-out test set (see notebook output).
- **Limitations:** only three features, one city, linear assumptions.

## Task 2 — Mall Customer Segmentation
- **Goal:** group customers by Annual Income and Spending Score.
- **Dataset:** Mall Customer Segmentation Data (Kaggle, 200 rows).
- **Method:** `StandardScaler`, Elbow Method + silhouette score, `KMeans` (K=5), cluster plot with centroids and cluster profiles.
- **Note:** clusters describe patterns in the chosen features, not fixed customer identities.

## How to run
1. Open a notebook in [Google Colab](https://colab.research.google.com) (File → Upload notebook, or open from GitHub).
2. Runtime → Run all. Datasets download automatically from public GitHub copies.
3. If a download fails, upload the CSV named in the notebook to the Colab file panel and re-run.

## Datasets and attribution
- Ames Housing: Dean De Cock (2011), via Kaggle.
- Mall Customers: Kaggle community dataset (vjchoudhary7).
