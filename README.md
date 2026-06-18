# Instacart Market Basket Analysis — Statistical EDA

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458)
![Seaborn](https://img.shields.io/badge/Seaborn-latest-4C72B0)
![License](https://img.shields.io/badge/License-Apache%202.0-green)

## Overview
This project performs a statistical exploratory data analysis on the 
Instacart Online Grocery dataset, which contains over 3 million orders 
from 200,000+ anonymous customers. The goal is to uncover meaningful 
patterns in customer purchasing behavior through descriptive statistics, 
distribution analysis, correlation, and variance computations.

**Dataset:** 5 tables — orders, products, order_products, aisles, departments  
**Tools:** Python, Pandas, Matplotlib, Seaborn

## Dataset
The dataset is sourced from the Instacart Market Basket Analysis competition 
on Kaggle. To download, visit [kaggle.com/c/instacart-market-basket-analysis](https://www.kaggle.com/c/instacart-market-basket-analysis/data).

## Project Structure
instacart-statistical-eda/
│

├── Instacart_Statistical_EDA.ipynb   # Main analysis notebook

└── README.md
## Analysis Summary

### Data Preprocessing
- Removed 15 duplicate records from the orders table
- Filled missing product names with 'Unknown'
- Replaced missing `add_to_cart_order` values with 999
- Standardized product names to lowercase

### Exploratory Data Analysis
| Section | Key Finding |
|---|---|
| Peak shopping hours | Orders peak between 10:00–16:00 |
| Busiest shopping days | Sunday and Monday have the highest order volumes |
| Reorder cycle | Most customers reorder on a 7-day cycle |
| Items per order | Typical basket contains 5–10 items |
| Top reordered items | Fresh produce dominates repeat purchases |

### Statistical Analysis
| Analysis | Finding |
|---|---|
| Mean order hour | ~13:45 — customers shop in early afternoon |
| Variance (order hour) | ~17.85 — moderate spread across hours |
| Mean days between orders | ~11 days |
| Correlation (dow vs hour) | ~0.008 — no significant relationship |

## Tools & Libraries
- **Python 3.x**
- **Pandas** — data manipulation and analysis
- **NumPy** — numerical operations
- **Matplotlib** — data visualization
- **Seaborn** — statistical data visualization

## How to Run
1. Clone the repository
```bash
git clone https://github.com/UghurKhalilov/instacart-statistical-eda.git
```
2. Open the notebook
```bash
jupyter notebook Instacart_Statistical_EDA.ipynb
```

## License
This project is licensed under the Apache License 2.0 — see the 
[LICENSE](LICENSE) file for details.
