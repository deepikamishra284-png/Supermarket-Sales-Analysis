# Supermarket Sales Analysis

**IBM SkillsBuild – Data Analytics with AI | Academic Internship Program**
Conducted by BharatCares in association with AICTE

**Author:** pp

## Project Overview
This project analyses 500 supermarket sales transactions (1 Jan – 1 Jul 2026) from four branches (Jaipur, Delhi, Mumbai, Bengaluru). It answers six business questions about products, branches, categories, payments, customer types and ratings, and turns the results into business recommendations.

## Dataset
- **File:** `supermarket_sales.csv` (included in this submission)
- **Link:** *add your Google Sheets / Drive / GitHub link here before submitting*
- **Size:** 500 rows × 13 columns
- **Columns:** Invoice ID, Date, Branch, City, Customer Type, Gender, Product, Category, Quantity, Unit Price, Payment, Rating, Sales
- **Data quality:** no missing values, no duplicates; `Sales = Quantity × Unit Price` holds for every row.

## Problem Statement
Analyse supermarket sales data to find useful information about products, branches, categories, customers, payments and ratings, and use it for business decisions.

## Key Findings
| Question | Answer |
|---|---|
| Highest-selling product | Cheese – ₹27,906.30 |
| Best branch | Branch C (Mumbai) – ₹72,469.45 |
| Top category | Beverages – ₹56,108.24 |
| Most popular payment | UPI – 127 transactions (all four methods are nearly equal) |
| Members vs Normal | Members ₹483.14 vs Normal ₹497.07 – Members do not spend more (not statistically significant) |
| Average rating | 3.99 / 5 |

Total sales: ₹2,44,411.08 | Average transaction: ₹488.82

## Technologies Used
Python 3 · Pandas · NumPy · Matplotlib · Seaborn · SciPy · Jupyter Notebook

## Project Structure
```
├── pp_Supermarket_Sales_Analysis.ipynb   # Analysis code with outputs
├── pp_ProjectReport.docx                 # Project report
├── requirements.txt                      # Dependencies
├── supermarket_sales.csv                 # Dataset
├── README.md
└── charts/                               # Created when the notebook runs
```

## Setup and Run
1. Install Python 3.9 or above.
2. (Optional) create a virtual environment:
   ```bash
   python -m venv venv
   venv\Scripts\activate        # Windows
   source venv/bin/activate     # macOS / Linux
   ```
3. Install the libraries:
   ```bash
   pip install -r requirements.txt
   ```
4. Keep `supermarket_sales.csv` in the same folder as the notebook, then start Jupyter:
   ```bash
   jupyter notebook pp_Supermarket_Sales_Analysis.ipynb
   ```
5. Choose **Kernel → Restart & Run All**. Charts are saved in the `charts/` folder.

## Business Recommendations (summary)
1. Keep strong stock of Cheese, Coffee, Shampoo and the Beverages, Personal Care and Dairy categories (about 60% of revenue).
2. Study Branch C's higher transaction volume and test its practices in Branch A (Jaipur).
3. Keep all payment methods active – usage is almost equal.
4. Add minimum-spend or bundle offers for Members to raise basket value.
5. Improve service, starting with Branch A (rating 3.84) and the ~23% of transactions rated below 3.5.

## Limitations
Small dataset (500 rows); July has only one day of data; no customer ID or profit data.
