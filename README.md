Market Basket Analysis using Apriori Algorithm

Project Overview

This project applies Market Basket Analysis to bakery transaction data to discover purchasing patterns and identify products that customers frequently buy together.

The main objective is to extract meaningful business insights using the Apriori algorithm and Association Rule Mining.

Dataset

The project uses the Bread Basket dataset, containing bakery sales transactions.

Total Records: 20,507

Unique Transactions: 9,465

Features: Transaction, Item, Date/Time, Period of Day, Weekday/Weekend.

Technologies & Libraries

Python

Pandas & NumPy

Matplotlib & Seaborn

MLxtend

Jupyter Notebook

Project Workflow

1. Data Cleaning & Preprocessing

Loaded and inspected the dataset.

Checked for missing values.

Converted date/time columns into appropriate formats.

Extracted date, month, hour, and weekday features.

Cleaned product names and standardized text formatting.

2. Exploratory Data Analysis (EDA)

Analyzed the most frequently purchased products.

Explored monthly and daily transaction patterns.

Analyzed purchasing behavior across different hours and periods of the day.

Visualized customer purchasing trends.

3. Market Basket Analysis

Applied the Apriori algorithm to identify frequent itemsets and discover associations between products.

Steps:

Transformed transaction data into a basket matrix.

Applied binary encoding (1 = item purchased, 0 = item not purchased).

Generated frequent itemsets using a minimum support threshold of 0.01.

Generated association rules using Lift with a minimum threshold of 1.

Ranked association rules based on Confidence.

4. Evaluation Metrics

The project uses three key metrics:

Support: Measures how frequently an itemset appears in all transactions.

Confidence: Measures how often the consequent is purchased when the antecedent is purchased.

Lift: Measures the strength of an association compared to what would be expected if the items were independent.

Key Findings

Coffee was the most frequently purchased product.

Purchasing activity was higher during weekends.

Afternoon hours showed significant purchasing activity.

Coffee appeared as a common associated product in several generated association rules.

The algorithm identified frequent combinations of products that can support cross-selling and product recommendation strategies.

Business Applications

Product recommendations.

Cross-selling strategies.

Product placement optimization.

Understanding customer purchasing behavior.

Supporting data-driven business decisions.

How to Run

Clone this repository:

git clone https://github.com/mohamedhazem14/market-basket-analysis-apriori.git

Install the required libraries:

pip install pandas numpy matplotlib seaborn mlxtend jupyter

Place the dataset file (bread basket.csv) in the project directory.

Open the Jupyter Notebook:

jupyter notebook apriori_algorithm_project.ipynb

Run all cells to reproduce the analysis.

Author

Mohamed Hazem Abdelghaffar

GitHub: https://github.com/mohamedhazem14

LinkedIn: https://www.linkedin.com/in/mohamed-hazem-74001a2b6/
