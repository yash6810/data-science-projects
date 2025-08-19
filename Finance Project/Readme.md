# 📊 Finance Data Project

This project is a **finance-focused data analysis project** designed to **strengthen your skills in data wrangling, time series analysis, and financial data visualization** using Python libraries like `pandas`, `pandas-datareader`, `matplotlib`, and `seaborn`.

> ⚠️ **Disclaimer**: This project is for **educational and practice purposes only**. It does **not constitute financial advice** or real-world investment recommendations.

---

## 🧠 Project Goal

To perform an **Exploratory Data Analysis (EDA)** on **major U.S. bank stocks** and analyze their performance:

- Before
- During
- After

the **2007–2008 Financial Crisis** through to early 2016.

The analysis highlights how bank stocks were affected over time, drawing attention to volatility, stock returns, moving averages, and sector-level comparisons.

---

## 📂 Dataset

- We use data from `pandas_datareader` to fetch **stock price data from Yahoo Finance**.
- The following banks are considered in this analysis:
  - Bank of America (BAC)
  - Citigroup (C)
  - Goldman Sachs (GS)
  - JPMorgan Chase (JPM)
  - Morgan Stanley (MS)
  - Wells Fargo (WFC)
- The file `all_banks.pkl` stores the entire collected and processed dataset in the form of a **multi-level column DataFrame** for ease of analysis.

---

## 🔍 Key Tasks Performed

### ✅ Data Collection
- Using `pandas_datareader` to fetch stock data from 2006 to 2016.

### ✅ Data Processing
- Merging all data into a single `pandas` DataFrame with **multi-index columns**.

### ✅ Visualization and Analysis
- **Line plots** of stock prices.
- **Rolling averages** and comparison with real prices.
- **Daily returns analysis** (percentage change).
- **Heatmaps and clustermaps** to identify correlation among banks.
- **Distplots** of stock returns and their risk profiles.
- **Cumulative returns plots** to measure long-term performance.

---

## 📈 Sample Code Preview

```python
import pandas as pd
from pandas_datareader import data as pdr
import datetime

start = datetime.datetime(2006, 1, 1)
end = datetime.datetime(2016, 1, 1)

BAC = pdr.DataReader('BAC', 'yahoo', start, end)
```

```python
tickers = ['BAC', 'C', 'GS', 'JPM', 'MS', 'WFC']
bank_stocks = pd.concat([pdr.DataReader(ticker, 'yahoo', start, end) for ticker in tickers], axis=1, keys=tickers)
```

---

## 🛠️ Technologies Used

- Python 3.x
- Jupyter Notebook
- pandas
- pandas-datareader
- matplotlib
- seaborn

---

## 📚 Learning Outcomes

By completing this project, I was able to gain practical experience with:
- Real-world **time series stock data**
- Working with **multi-level indexed DataFrames**
- Advanced **pandas** operations like `xs()`, `pct_change()`, `rolling()`
- Building **interactive plots** and **heatmaps**
- Understanding stock return distributions and correlation structures

---

## ▶️ How to Run

1. Install the required libraries:
   ```bash
   pip install pandas pandas-datareader matplotlib seaborn
   ```
2. Open the notebook `03-Finance Project.ipynb` in Jupyter.
3. Run all the cells sequentially.
4. Explore visualizations and insights step-by-step.

---

## 📎 Project Structure

```
├── 03-Finance Project.ipynb     # Main Jupyter Notebook
├── all_banks.pkl                # Processed DataFrame of all stock data
└── README.md                    # Project documentation
```

---

## ✍️ Author & Credits
Author: Yash Upadhyay
📧 Email: yashupadhyay481@gmail.com
🔗 [LinkedIn](www.linkedin.com/in/yash-upadhyay-309b44281) | [GitHub](https://github.com/yash6810)

This project is based on the **Pierian Data** curriculum, adapted for personal practice and demonstration. Logo and resources © [Pierian Data](http://www.pieriandata.com)

---

## 📌 References

- [Yahoo Finance](https://finance.yahoo.com/)
- [Pandas DataReader Documentation](https://pydata.github.io/pandas-datareader/)
- [2007–08 Financial Crisis - Wikipedia](https://en.wikipedia.org/wiki/Financial_crisis_of_2007%E2%80%9308)

