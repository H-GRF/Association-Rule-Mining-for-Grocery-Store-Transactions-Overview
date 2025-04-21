
# Association Rule Mining for Grocery Store Transactions

## Overview
This project applies **Association Rule Mining** to analyze transaction data from a grocery store using the **Apriori algorithm**. The goal is to uncover relationships between different products bought together by customers, also known as **market basket analysis**. The analysis helps identify frequent itemsets, which can be used for **recommendation systems**, **inventory management**, and improving marketing strategies.

## Objective
The objective of this project is to:
1. Apply the **Apriori algorithm** to identify frequent itemsets in the grocery store dataset.
2. Generate **association rules** based on these itemsets to discover product relationships.
3. Evaluate these rules using key metrics: **Support**, **Confidence**, and **Lift**.

## Approach

1. **Data Preprocessing**: The dataset consists of transactions where each row represents a list of products bought together. The first step is to convert the dataset into a format suitable for applying the Apriori algorithm (e.g., one-hot encoding for each item).
   
2. **Frequent Itemset Mining**: Using the Apriori algorithm, frequent itemsets are identified. These are groups of items that frequently appear together in customer transactions.
   
3. **Association Rule Generation**: From the frequent itemsets, association rules are generated. These rules describe relationships like "if a customer buys X, they are likely to also buy Y."

4. **Evaluation of Rules**: The generated rules are evaluated using the following metrics:
   - **Support**: The proportion of transactions containing the itemset.
   - **Confidence**: The likelihood that an item Y is bought when item X is bought.
   - **Lift**: The ratio of observed support to expected support if X and Y were independent.

## Dataset Description
The dataset consists of transaction records from a grocery store, where each transaction contains a list of items bought together. Here is an example of how the data looks:

| Transaction ID | Items                                             |
|----------------|---------------------------------------------------|
| 1              | BREAD, MILK, BISCUIT, CORNFLAKES                 |
| 2              | BREAD, TEA, BOURNVITA                            |
| 3              | JAM, MAGGI, BREAD, MILK                          |
| 4              | MAGGI, TEA, BISCUIT                              |

### Key Columns:
- **Items**: List of products bought together in a transaction.

## Files in the Repository
- **association-rules.ipynb**: Jupyter notebook that contains the implementation of the Apriori algorithm, association rule generation, and rule evaluation.
- **GroceryStoreDataSet.csv**: CSV file containing the transaction data from the grocery store.
- **association-rules.tar.gz**: A compressed file that may contain additional resources or files related to the project.

## How to Run the Project

### 1. Clone the Repository:
```bash
git clone https://github.com/your-username/repository-name.git
```

### 2. Install Dependencies:
Install required Python libraries:
```bash
pip install -r requirements.txt
```

### 3. Run the Jupyter Notebook:
Open the Jupyter notebook using Jupyter Notebook or JupyterLab:
```bash
jupyter notebook association-rules.ipynb
```

### 4. Explore the Dataset:
Load and explore the dataset to understand customer transactions and perform data preprocessing.

### 5. Apply Apriori Algorithm:
Run the cells to apply the Apriori algorithm, generate frequent itemsets, and extract association rules.

### 6. Evaluate the Rules:
Examine the **Support**, **Confidence**, and **Lift** metrics to assess the quality of the generated rules.

## Conclusion
This project provides valuable insights into customer behavior by uncovering patterns and associations between different products in the grocery store. The association rules can be used to inform business decisions such as promotional strategies, cross-selling opportunities, and inventory management.

