# Data-Science-Assignment
Certainly! Here’s a more detailed version of the `README.md` for your GitHub repository:

---

# Data Science Assignment: eCommerce Transactions Dataset

## Overview

This repository contains the solution for a data science assignment based on an eCommerce transactions dataset. The dataset consists of three primary files: `Customers.csv`, `Products.csv`, and `Transactions.csv`. The task was to perform detailed exploratory data analysis (EDA), build a lookalike model, and implement clustering techniques to segment customers based on both their profile and transaction data.

This assignment aims to demonstrate skills in data manipulation, exploratory analysis, machine learning model development, and deriving actionable business insights from data.

---

## Dataset Files

The dataset includes the following files:

1. **Customers.csv**:
   - `CustomerID`: Unique identifier for each customer.
   - `CustomerName`: Name of the customer.
   - `Region`: The continent or region where the customer resides.
   - `SignupDate`: The date when the customer signed up for the platform.

2. **Products.csv**:
   - `ProductID`: Unique identifier for each product.
   - `ProductName`: Name of the product.
   - `Category`: The category to which the product belongs (e.g., Electronics, Apparel, etc.).
   - `Price`: The price of the product in USD.

3. **Transactions.csv**:
   - `TransactionID`: Unique identifier for each transaction.
   - `CustomerID`: The ID of the customer who made the transaction.
   - `ProductID`: The ID of the product sold in the transaction.
   - `TransactionDate`: The date when the transaction took place.
   - `Quantity`: The number of units of the product purchased.
   - `TotalValue`: The total value of the transaction (calculated as Quantity * Price).
   - `Price`: The price at which the product was sold.

---

## Assignment Tasks

### Task 1: Exploratory Data Analysis (EDA) and Business Insights

**Objective**: Perform a thorough EDA on the dataset and generate at least 5 actionable business insights.

#### Steps Taken:
- Explored the dataset to understand the data types, missing values, and basic statistics.
- Performed data cleaning (handling missing values, duplicates, etc.).
- Conducted univariate and bivariate analyses to uncover patterns, correlations, and distributions in the data.
- Created visualizations (bar plots, histograms, heatmaps) to better understand key data characteristics.

#### Insights Generated:
- Derived at least 5 business insights, focusing on customer behavior, product popularity, and regional trends.
- The insights were aimed at helping eCommerce businesses understand their customer demographics, identify popular products, and tailor marketing strategies accordingly.

#### Deliverables:
- **Jupyter Notebook**: `EDA.ipynb` containing the code for data exploration and visualizations.
- **PDF Report**: `EDA.pdf` containing the summarized business insights.

### Task 2: Lookalike Model

**Objective**: Develop a Lookalike Model that takes a customer's profile and transaction history as input and recommends 3 similar customers.

#### Steps Taken:
- Combined customer profile information (e.g., Region, SignupDate) with transaction history (e.g., product categories, frequency of purchases).
- Preprocessed the data to prepare it for similarity calculations using customer profiles and transaction patterns.
- Built a model using a similarity scoring approach (e.g., cosine similarity or a weighted scoring system) to recommend similar customers.
- Selected the top 3 similar customers for each of the first 20 customers.

#### Deliverables:
- **Lookalike Model Output**: `Lookalike.csv` containing the top 3 lookalikes for customers C0001 - C0020, along with their similarity scores.
- **Jupyter Notebook**: `Lookalike_Model.ipynb` explaining the model development and similarity scoring process.

### Task 3: Customer Segmentation / Clustering

**Objective**: Perform customer segmentation using clustering techniques on both customer profiles and transaction information.

#### Steps Taken:
- Used both customer demographic data and transaction data to cluster customers.
- Applied clustering algorithms such as **K-Means**, **DBSCAN**, or **Hierarchical Clustering** to segment customers into distinct groups.
- Evaluated the clustering model using metrics like the **Davies-Bouldin Index** (DB Index) and visualized the clusters using 2D plots (e.g., PCA or t-SNE for dimensionality reduction).

#### Deliverables:
- **Clustering Report**: `Clustering.pdf` containing an in-depth analysis of the clusters, DB Index value, and insights from the clustering model.
- **Jupyter Notebook**: `Clustering.ipynb` containing the code for clustering and the evaluation metrics used.

---

## Installation

To run the code and replicate the results in this repository, you'll need Python along with the following libraries:

- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- scipy
- sklearn
- plotly (optional for advanced visualizations)

You can install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## Folder Structure

The folder structure for this repository is as follows:

```
├── Customers.csv               # Customer data
├── Products.csv                # Product data
├── Transactions.csv            # Transaction data
├── SaiVignesh_Thiruvidhula_EDA.ipynb                   # Jupyter notebook for Exploratory Data Analysis
├── SaiVignesh_Thiruvidhula_Lookalike_Model.ipynb       # Jupyter notebook for Lookalike Model development
├── SaiVignesh_Thiruvidhula_Clustering.ipynb            # Jupyter notebook for Customer Segmentation using Clustering
├── SaiVignesh_Thiruvidhula_EDA.pdf                     # PDF report containing business insights
├── SaiVignesh_Thiruvidhula_Lookalike.csv               # Output of the Lookalike Model with similarity scores
├── SaiVignesh_Thiruvidhula_Clustering.pdf              # PDF report with clustering results
└── requirements.txt            # List of dependencies
```

---

---

## Results and Conclusion

The analysis provided insights into:
- Key customer demographics and purchasing patterns.
- Identifying similar customers using a lookalike model.
- Segmenting customers based on their profiles and transaction behaviors, which can be used for personalized marketing, product recommendations, and targeted campaigns.

The final submission demonstrates the effective use of machine learning algorithms, clustering techniques, and exploratory data analysis to extract actionable insights that can benefit an eCommerce business.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- Data source: eCommerce Transactions dataset.
- Libraries and tools used: pandas, numpy, scikit-learn, matplotlib, seaborn.

---

This detailed `README.md` file not only provides a clear description of each task and deliverable but also guides users through the repository structure, the steps you followed, and the tools used. It ensures that anyone accessing your project can understand the objectives, methods, and results, even if they are unfamiliar with the original dataset or the context of the assignment.
