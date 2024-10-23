# Big Data Analysis of Online Retail Transactions

**Overview**

This project focuses on analyzing an online retail dataset to derive valuable insights about customer purchasing behaviors and product trends. Utilizing PySpark for data manipulation and H2O for machine learning, the analysis aims to segment customers based on their buying preferences and predict customer segments for improved marketing strategies.

**Dataset**

The dataset used in this project is sourced from the UCI Machine Learning Repository and contains transaction records from an online retail store. Key attributes include:

- Description: The name of the product.
- Quantity: The quantity of each product sold.
- UnitPrice: The price per unit of the product.
- CustomerID: A unique identifier for each customer.
- InvoiceDate: The date and time of the transaction.

**Key Steps**

  # Data Loading and Exploration
  
The dataset was loaded using the ucimlrepo package, and initial exploration was performed to understand its structure and contents.
Missing values were handled, particularly in the Description and CustomerID columns.

*Data Preprocessing*
The Description column was transformed to lowercase for consistency.
Tokenization was applied to convert product descriptions into a list of words.
Unique products and their total quantities were calculated to identify the most popular items.
*Customer Analysis*
Unique customer counts were calculated, and payments were aggregated to identify total spending by each customer.
A SQL query was utilized to find the top products sold by country.
Customers were segmented into two groups based on their purchasing preferences—one group that buys in bulk at lower prices and another group that prefers high-quality items in smaller quantities.
*Sales Analysis*
The dataset was enriched with features such as total sales by hour and by season, enabling insights into purchasing trends over time.
Visualizations were created to illustrate total sales by hour and season.
Feature Engineering
Various features were combined to create a comprehensive dataset for machine learning modeling, including customer segments, temporal features, and textual representations of product descriptions.
*Modeling*
The H2O framework was employed to create predictive models using deep learning and random forests to classify customers into segments.
A grid search was conducted to optimize hyperparameters for a gradient boosting model, improving model performance.
*Visualization*
Matplotlib and Seaborn were used for data visualization to provide insights into customer purchasing behavior, product trends, and correlations between features.

**Conclusion**

The project demonstrates the application of big data technologies in analyzing retail transactions. By segmenting customers and predicting their preferences, businesses can tailor their marketing strategies and improve customer engagement.

Leveraging PySpark to analyze and extract insights from large-scale online retail data, focusing on consumer behavior, product performance, and sales trends.
