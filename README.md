# ** MAT 455: Data Analysis Project
## **House Prices in Ames, Iowa**
### **Spring 2025**
#### **Student Name: Asifur Rahman **

---

## **Abstract**

The housing market plays a critical role in the economy, influencing both individual wealth and broader financial stability. This project aims to analyze house prices in Ames, Iowa, using statistical methods to identify key factors that affect home values. The dataset, sourced from publicly available real estate data, includes variables such as lot size, square footage, number of bedrooms, year built, and neighborhood. Through a combination of regression modeling, classification techniques, forcasting houses price and exploratory data analysis, this study will evaluate the relationships between property characteristics and sale prices. The findings will provide insights into price determinants and help in forecasting property values, which is beneficial for homeowners, buyers, and real estate investors.

---

## **Chapter 1: Introduction**

Real estate pricing is a complex subject influenced by multiple factors, such as location, property characteristics, and market trends. Understanding these factors is crucial for buyers, sellers, and policymakers. The primary objective of this study is to analyze house price variations in Ames, Iowa, using statistical methodologies. This study seeks to answer the following questions:

1. What are the key determinants of house prices in Ames, Iowa?
2. How do different statistical techniques compare in predicting house prices?
3. What role do categorical variables such as neighborhood and house style play in price variation?
4. How does the price of houses vary by area and neighborhood?
5. What impact do structural features like number of rooms, total SF on pricing treands?
6. Are there seasonal treands in house pricing within the dataset?

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

| Feature       | Mean  | Median | Std Dev | Min  | Max |
|--------------|-------|--------|---------|------|------|
| SalePrice    | 180921 | 163000 | 79442   | 34900 | 755000 |
| LotArea      | 10168  | 9478   | 7886    | 1300  | 215245 |
| GrLivArea    | 1515   | 1442   | 525     | 334   | 5642 |

### **Preliminary Data Visualization**
Several visualizations will be conducted to better understand relationships within the data. Some initial findings include:
- A positive correlation between **GrLivArea** and **SalePrice**.
- A strong relationship between **OverallQual** and **SalePrice**.
- Higher house prices in neighborhoods such as **StoneBr**, **NridgHt**, and **NoRidge**.

By applying appropriate statistical techniques, this project aims to develop a robust model for predicting house prices in Ames, Iowa.

---

### **Next Steps**

- Implement statistical models (linear regression, classification, resampling methods).
- Perform in-depth data analysis and hypothesis testing.
- Compare different modeling approaches and determine the best predictive model.
- Interpret and present findings in a meaningful way.


