# 🛒 Market Basket Analysis | Apriori Algorithm

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/MLxtend-Apriori-orange" />
  <img src="https://img.shields.io/badge/Domain-Data%20Science-success" />
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen" />
</p>

## 📌 Project Overview

This project focuses on **Market Basket Analysis (MBA)** using bakery transaction data to uncover customer purchasing patterns and discover products that are frequently purchased together.

Using the **Apriori Algorithm** and **Association Rule Mining**, the project identifies meaningful relationships between products and transforms transaction data into actionable business insights.

The goal is to understand customer purchasing behavior and demonstrate how data mining techniques can support smarter business decisions.

## 📂 Dataset

The project uses the **Bread Basket Dataset**, which contains historical bakery sales transactions.

| Dataset Information | Details |
|---|---|
| Total Records | 20,507 |
| Unique Transactions | 9,465 |
| Data Type | Transactional Data |
| Domain | Retail / Bakery Sales |

**Main Features:**
- `Transaction` – Unique transaction identifier.
- `Item` – Purchased product.
- `DateTime` – Transaction date and time.
- `Period of Day` – Time period of the transaction.
- `Weekday/Weekend` – Day classification.

## 🛠️ Tech Stack & Libraries

| Technology | Purpose |
|---|---|
| 🐍 Python | Core programming language |
| 🐼 Pandas | Data manipulation and analysis |
| 🔢 NumPy | Numerical operations |
| 📊 Matplotlib | Data visualization |
| 🎨 Seaborn | Statistical visualization |
| 🔍 MLxtend | Apriori algorithm and association rules |
| 📓 Jupyter Notebook | Development environment |

## ⚙️ Project Workflow

### 1️⃣ Data Cleaning & Preprocessing
- Loaded and inspected the dataset.
- Checked for missing values and data quality issues.
- Converted date/time columns into appropriate formats.
- Extracted date, month, hour, and weekday features.
- Cleaned product names and standardized text formatting.

### 2️⃣ Exploratory Data Analysis (EDA)
- Identified the most frequently purchased products.
- Analyzed monthly and daily transaction patterns.
- Explored customer purchasing behavior across different hours.
- Compared purchasing activity across different periods of the day.
- Created visualizations to understand sales trends and patterns.

### 3️⃣ Market Basket Analysis (Apriori)

Applied the **Apriori Algorithm** to discover frequent itemsets and generate association rules.

**Implementation Steps:**

- Transformed transactional data into a basket matrix.
- Applied binary encoding:
  - `1` = Item purchased.
  - `0` = Item not purchased.
- Generated frequent itemsets using a minimum support threshold of `0.01`.
- Generated association rules using Lift with a minimum threshold of `1`.
- Ranked the generated rules based on Confidence.

## 📐 Association Rule Metrics

Three important metrics were used to evaluate product associations:

| Metric | Description |
|---|---|
| **Support** | Measures how frequently an itemset appears across all transactions. |
| **Confidence** | Measures how often the consequent is purchased when the antecedent is purchased. |
| **Lift** | Measures the strength of an association compared to what would be expected if the items were independent. |

**Understanding Lift:**
- `Lift > 1` → Positive association.
- `Lift = 1` → Items are independent.
- `Lift < 1` → Negative association.

## 📊 Key Findings & Insights

The analysis revealed several interesting patterns:

- ☕ **Coffee** was the most frequently purchased product.
- 📅 Purchasing activity was higher during weekends.
- 🕒 Afternoon hours showed significant purchasing activity.
- 🛍️ Coffee appeared as a common associated product in several generated association rules.
- 🔗 The Apriori algorithm identified frequent product combinations that can help businesses understand customer preferences.

## 💡 Business Applications

The insights generated from this project can support several business strategies:

- 🎯 **Product Recommendations:** Suggest related products based on purchasing patterns.
- 🛒 **Cross-Selling:** Encourage customers to purchase complementary products.
- 🏪 **Product Placement:** Optimize product positioning based on customer buying behavior.
- 📈 **Business Intelligence:** Support data-driven decisions using transaction data.
- 👥 **Customer Behavior Analysis:** Understand purchasing habits and product relationships.

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/mohamedhazem14/market-basket-analysis-apriori.git
```

### 2. Navigate to the Project Directory

```bash
cd market-basket-analysis-apriori
```

### 3. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn mlxtend jupyter
```

### 4. Prepare the Dataset

Place the `bread basket.csv` dataset in the project directory.

### 5. Launch Jupyter Notebook

```bash
jupyter notebook market_basket_analysis.ipynb
```

Run all cells to reproduce the analysis and generate the results.

## 📁 Project Structure

```text
market-basket-analysis-apriori/
│
├── market_basket_analysis.ipynb
├── bread basket.csv
├── README.md
├── LICENSE
└── .gitignore
```

## 👨‍💻 Author

**Mohamed Hazem Abdelghaffar**

🎓 Computer Science Graduate | Data Science

Interested in Data Science, Machine Learning, Artificial Intelligence, and Data Engineering.

<p align="left">
  <a href="https://github.com/mohamedhazem14">
    <img src="https://img.shields.io/badge/GitHub-Profile-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
  <a href="https://www.linkedin.com/in/mohamed-hazem-74001a2b6/">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
</p>

---

⭐ If you find this project useful, feel free to star the repository!
