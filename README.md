# Kindle Book Success Analysis

> Analyzing how publisher reputation and cover design influence book sales, ratings, and bestseller status in the digital marketplace — built with Python, Pandas, Seaborn, and statistical modeling on a structured Kindle dataset.

---

## Project Overview

This project investigates the key factors that drive a book's commercial success on Amazon Kindle. Using a structured Kindle book dataset, the analysis examines how publisher reputation (e.g., Penguin, HarperCollins) and cover design attributes interact with sales performance, customer ratings, and review engagement.

The findings provide actionable guidance for publishers, authors, and investors seeking to optimize their digital marketplace strategy.

**Tools & Technologies:** Python · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn · Jupyter Notebook

---

## Research Questions

1. How does publisher reputation affect a book's sales performance, rating, and reviews?
2. How does a book's cover design contribute to success across different categories?
3. What is the relationship between book price and customer review engagement?
4. Which factors most strongly predict bestseller status?

---

## Key Findings

- **Publisher reputation is the strongest driver of success** — books from Penguin and HarperCollins consistently achieve higher ratings, more reviews, and greater bestseller rates due to audience trust and superior marketing reach
- **Cover design matters differently by genre** — minimalist covers perform best in non-fiction, while bold and vibrant designs correlate with success in fiction
- **Sweet spot pricing ($5–$15)** generates the highest volume of customer reviews, as readers perceive it as the best price-to-value ratio
- **Bestselling books show consistently higher and more uniform ratings** than non-bestsellers, confirming that reader trust reinforces commercial momentum
- **Price alone is a weak predictor of sales success** — publisher brand and editorial quality outweigh pricing as a success factor

---

## Dataset

- **Source:** Kindle book dataset (kindle_data-v2.csv)
- **Key fields:** Title, Author, Publisher, Category, Price, Stars (Rating), Reviews, Bestseller Status, Editor's Pick, Kindle Unlimited, Published Year
- **Size:** Large structured dataset with multiple performance indicators per book

---

## Methodology

### 1. Data Cleaning & Preprocessing
- Filled missing author names with "Unknown Author" placeholder
- Imputed missing publisher/seller values with the most frequent value
- Extracted `publishedYear` from dates and dropped the raw date column
- Detected and removed outliers in price and review counts

### 2. Feature Engineering
- Normalized price and review counts to [0, 1] range using MinMaxScaler
- Created category-level bestseller frequency statistics
- Engineered normalized rating variables for cross-category comparison

### 3. Statistical Analysis
- Descriptive statistics (mean, median, distribution) for price, rating, and reviews
- Correlation matrix to identify relationships between all numerical variables
- Publisher-level performance comparison

### 4. Visualization
- **Histogram** — distribution of normalized book prices
- **Box plot** — review count distribution and outlier detection
- **Correlation heatmap** — relationships between price, rating, reviews, and bestseller status
- **Pair plot** — pairwise relationships across all key variables

---

## Results Summary

| Factor | Impact on Success |
|---|---|
| Publisher reputation (Penguin, HarperCollins) | Strong positive — higher ratings, reviews, bestseller rate |
| Cover design (professional typography + color) | Positive — increases visibility and customer interest |
| Price range $5–$15 | Highest review engagement |
| High ratings | Strong predictor of bestseller status |
| Price alone | Weak predictor — not a reliable success factor |

---

## Repository Structure

```
├── Code.ipynb                        # Main analysis notebook
├── FCSS_Project_Report.pdf           # Full research report
├── Poster.pdf                        # Visual project summary poster
└── kindle_data-v2.csv                # Dataset
```

---

## How to Run

```bash
# Clone the repository
git clone https://github.com/Mahmudul-Hasan-24/Kindle-Book-Success-Analysis-Python.git

# Install required packages
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# Launch the notebook
jupyter notebook Code.ipynb
```

---

## Skills Demonstrated

- Data cleaning and preprocessing (missing values, outlier removal, normalization)
- Feature engineering with Scikit-learn (MinMaxScaler)
- Exploratory data analysis (EDA) and statistical modeling
- Multi-variable correlation analysis
- Data visualization with Matplotlib and Seaborn
- Translating analytical findings into business recommendations

---

## Author

**Mahmudul Hasan**
M.Sc. Computational Social Systems (Business Analytics)
Technical University of Graz & University of Graz
[LinkedIn](https://www.linkedin.com/in/mahmudul-hasan-764307249/) · [GitHub](https://github.com/Mahmudul-Hasan-24)
