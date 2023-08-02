# Project description

In this code, the objective is to perform Market Basket Analysis on transaction data to identify association rules between different product categories. The dataset contains information about orders and products, and we use the Apriori algorithm to identify frequent itemsets and then generate association rules.

Here is a step-by-step breakdown of the code:

Import necessary modules: The code starts by importing required libraries, including NumPy, pandas, matplotlib, plotly, and mlxtend modules.

Load data: Three datasets are loaded using the pandas read_csv() function: "orders," "products," and "translations."

Data Preparation: The "products" dataset is translated into English using the "translations" dataset to improve data readability. Additionally, the "product_category_name_english" column is added to the "orders" dataset.

Check for Missing Data: The code checks for missing data in the "orders" dataset and drops rows with missing "product_category_name_english" values.

Data Exploration: The code explores the number of unique products and product categories in the dataset.

Construct Transactions: The "transactions" are constructed by grouping all items in each order.

One-Hot Encoding: One-hot encoding is applied to convert the transaction data into a binary matrix.

Compute Metrics: The code computes support and confidence metrics for different itemsets.

Association Rules and Pruning: The Apriori algorithm is applied to identify frequent itemsets, and then association rules are generated using a specified confidence threshold.

The code successfully prepares the data and performs Market Basket Analysis to find meaningful association rules between different product categories based on the transactions data. The association rules indicate the likelihood of purchasing certain product categories when others are bought, which can be valuable for cross-selling and marketing strategies.

# Dataset description
The dataset used for this project is a Brazillian E-commerce dataset of orders made at Olist store sourced from Kaggle

# Tech/Libraries used
pandas
matplotlib
plotly
mlxtend
