

# MAT 455: Data Analysis Project
## **House Prices in Ames, Iowa**
### **Spring 2025**
#### **Student Name: Asifur Rahman**

---

## **Abstract**

The housing market plays a critical role in the economy, influencing both individual wealth and broader financial stability. This project aims to analyze house prices in Ames, Iowa, using statistical methods to identify key factors that affect home values. The dataset, sourced from publicly available real estate data, includes variables such as lot size, square footage, number of bedrooms, year built, and neighborhood. Through a combination of regression modeling, classification techniques, forecasting house prices, and exploratory data analysis, this study will evaluate the relationships between property characteristics and sale prices. The findings will provide insights into price determinants and help in forecasting property values, which is beneficial for homeowners, buyers, and real estate investors.

---

## **Chapter 1: Introduction**

Real estate pricing is a complex subject influenced by multiple factors, such as location, property characteristics, and market trends. Understanding these factors is crucial for buyers, sellers, and policymakers. The primary objective of this study is to analyze house price variations in Ames, Iowa, using statistical methodologies. This study seeks to answer the following questions:

1. What are the key determinants of house prices in Ames, Iowa?
2. How do different statistical techniques compare in predicting house prices?
3. What role do categorical variables such as neighborhood and house style play in price variation?
4. How does the price of houses vary by area and neighborhood?
5. What impact do structural features like number of rooms, total SF have on pricing trends?
6. Are there seasonal trends in house pricing within the dataset?

The project leverages regression models, classification techniques, and resampling methods to build predictive models and interpret significant factors influencing house prices. The analysis will be useful for real estate professionals, investors, and policymakers in making data-driven decisions.

---

## **Chapter 2: Data Description**

The dataset used in this study is the **Ames Housing Dataset**, originally compiled by Dean De Cock for educational purposes. It contains detailed information on over 2,900 houses sold in Ames, Iowa, between 2006 and 2010. The dataset includes 82 variables describing various aspects of residential homes, such as:

- **SalePrice**: The target variable representing the sale price of the house.
- **LotArea**: Total size of the lot (square feet).
- **OverallQual**: Overall material and finish quality.
- **YearBuilt**: Year the house was built.
- **GrLivArea**: Above-ground living area (square feet).
- **Neighborhood**: The physical location of the property within Ames.
- **GarageCars**: Number of cars that fit in the garage.
- **TotalBsmtSF**: Total basement square footage.

### **Data Collection and Processing**

The dataset is publicly available and has been preprocessed to remove duplicates and missing values. The following steps were taken to prepare the data:

- **Handling Missing Data**: Columns with missing values were analyzed, and appropriate imputation techniques were applied.
- **Data Cleaning**: Outliers were identified and treated to prevent distortion of results.
- **Exploratory Data Analysis (EDA)**: Visualizations and summary statistics were used to understand the data distribution.
- **Feature Engineering**: Certain variables were transformed or combined to improve predictive performance.

Below are some key statistical summaries:

| Feature       | Mean    | Median  | Std Dev | Min   | Max     |
|--------------|---------|---------|---------|-------|---------|
| SalePrice    | 180,921 | 163,000 | 79,442  | 34,900| 755,000 |
| LotArea      | 10,168  | 9,478   | 7,886   | 1,300 | 215,245 |
| GrLivArea    | 1,515   | 1,442   | 525     | 334   | 5,642   |

### **Preliminary Data Visualization**

Several visualizations were conducted to better understand relationships within the data. Some initial findings include:

- A positive correlation between **GrLivArea** and **SalePrice**.
- A strong relationship between **OverallQual** and **SalePrice**.
- Higher house prices are observed in neighborhoods such as **StoneBr**, **NridgHt**, and **NoRidge**.

---

## **Chapter 3: Modeling and Evaluation**

Multiple regression models were trained and evaluated to identify the best predictive algorithm. Models included linear approaches, regularization techniques, and tree-based ensemble methods. Below is a summary of their performance:

| Model              | R² Score | RMSE       |
|--------------------|-----------|------------|
| XGBoost            | 0.9152    | 21,500.23  |
| LightGBM           | 0.9128    | 21,780.12  |
| Random Forest      | 0.9101    | 22,000.55  |
| Lasso              | 0.8995    | 23,400.00  |
| Ridge              | 0.8979    | 23,582.00  |
| Linear Regression  | 0.8900    | 23,491.00  |
| Gradient Boosting  | 0.9050    | 22,550.34  |
| ElasticNet         | 0.8788    | 25,698.00  |
| MLP Regressor      | 0.8502    | 27,500.89  |
| SVR                | 0.7904    | 30,500.99  |

### **Best Model: XGBoost**
XGBoost showed the best performance, achieving the highest R² and lowest RMSE. It handles multicollinearity well and is robust to outliers and nonlinear relationships.

---

## **Chapter 4: Conclusion and Next Steps**

The project successfully identified key factors influencing house prices in Ames, Iowa. Among the models tested, XGBoost was the most accurate. Key takeaways include:

- **Overall Quality**, **Living Area**, **Garage Capacity**, and **Basement Size** are strong predictors.
- Neighborhood plays a crucial role in price variation.
- Regularization (Lasso, Ridge) helps manage overfitting but is slightly less accurate than tree-based models.

### **Next Steps**

- Conduct residual diagnostics and error analysis on XGBoost predictions.
- Deploy the model using Flask or Streamlit for interactive use.
- Perform time-based analysis to explore seasonal or yearly pricing trends.
- Extend analysis to include external economic factors or interest rate data for forecasting.

---

## **Appendix**

The complete notebooks `EDA.ipynb` and `FE_and_modeling.ipynb` contain the code, visualizations, and feature transformations used in this study.

---

## **Author**

**Asifur Rahman**  
MAT 455: Applied Statistics / Data Analysis  
Spring 2025  
John Jay College of Criminal Justice
