# Supermarket Sales Analytics and Prediction System

## Project Overview
This project performs end-to-end data analysis and machine learning on supermarket product sales data. It includes data cleaning, preprocessing, statistical analysis, visualization, customer segmentation, clustering, and predictive modeling to generate business insights and sales predictions.

This project demonstrates a complete real-world data analytics pipeline starting from raw data to machine learning model evaluation.

---

## Objectives
- Clean and preprocess raw supermarket sales data
- Perform exploratory data analysis (EDA)
- Identify customer purchasing patterns
- Segment customers based on sales behavior
- Build predictive models for sales forecasting
- Generate business insights for decision making

---

## Dataset Information

### Files Used
- `supermarket_product.csv` – Raw dataset
- `supermarket_product_cleaned.csv` – Cleaned dataset after preprocessing

### Key Columns
- Item Identifier
- Item Weight
- Item Fat Content
- Item Visibility
- Item Type
- Item MRP
- Outlet Identifier
- Outlet Establishment Year
- Outlet Size
- Outlet Location Type
- Outlet Type
- Item Outlet Sales

---

## Technology Stack

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Scikit-learn

---

## Data Preprocessing

### Missing Value Handling
- Numerical columns filled using median values
- Categorical columns filled using mode values

### Outlier Removal
- Used Interquartile Range (IQR) method to remove extreme values

### Feature Engineering
Created new features including:
- Outlet Age (Current Year – Establishment Year)
- Discount estimation feature
- Repeated Sales (Mean sales per item)
- Customer Value Category (High, Mid, Low based on quantiles)

---

## Statistical Analysis
Performed statistical analysis on sales data including:
- Mean and Median
- Standard Deviation and Variance
- Range
- Interquartile Range (IQR)
- Skewness
- Kurtosis
- Z-score standardization

---

## Exploratory Data Analysis and Visualization
Visualizations created:
- Sales distribution histogram
- Sales trend across establishment years
- Price vs Sales demand scatter plot
- Sales frequency distribution
- Product category vs outlet performance heatmap
- Regional sales comparison
- Correlation heatmap of numerical variables
- Discount vs Sales regression visualization

---

## Customer Segmentation

### Quantile Based Segmentation
Customers/items categorized into:
- High Value
- Mid Value
- Low Value

### Clustering
- K-Means clustering applied
- Elbow method used to determine optimal number of clusters
- Segmentation based on Item MRP and Item Outlet Sales

---

## Machine Learning Models

### Simple Linear Regression
Target Variable:
- Item Outlet Sales

Feature Used:
- Item MRP

Performance:
- R-squared approximately 0.30

---

### Multiple Linear Regression
Features Used:
- Item MRP
- Outlet Age
- Item Fat Content (Encoded)
- Outlet Type (Encoded)

Performance:
- R-squared improved to approximately 0.49 after data cleaning and feature engineering
- Mean Squared Error reduced compared to simple regression

---

## Advanced Analysis

### Regression Toward the Mean Study
- Calculated repeated sales mean per item
- Compared initial sales vs average sales
- Calculated sales deviation

### Correlation Analysis
- Discount vs Sales showed strong negative correlation
- Repeated Sales vs Actual Sales showed strong positive relationship

---

## Key Business Insights
- Pricing has moderate influence on sales performance
- Higher discount values correlate with lower effective sales outcomes
- Outlet characteristics influence sales patterns
- Customer purchase behavior can be segmented effectively using clustering

---

## Results Summary
- Cleaned dataset prepared for modeling
- Customer segments successfully identified
- Machine learning model built for sales prediction
- Multiple regression model significantly improved prediction accuracy

---

## Future Improvements
- Implement advanced models such as Random Forest or Gradient Boosting
- Deploy model using Streamlit dashboard
- Integrate real-time sales prediction
- Connect with Power BI for enterprise reporting
- Expand dataset with time-series sales data

---

## How to Run the Project

### Install Required Libraries
pip install pandas numpy matplotlib seaborn scikit-learn scipy

