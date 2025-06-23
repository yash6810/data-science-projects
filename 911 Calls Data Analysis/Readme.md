# 🚨 911 Calls Data Analysis – Capstone Project

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Status](https://img.shields.io/badge/Project-Complete-brightgreen.svg)]()

A data analysis and visualization project on real 911 emergency call logs from Montgomery County, PA. The project explores patterns in emergency services usage to uncover key trends by reason, time, and location using Python and data science libraries.

---

## 📂 Project Overview

This capstone project walks through the full lifecycle of a real-world dataset — from loading and cleaning to visual analysis. We explore the types and frequency of emergency calls, identify peak hours and locations, and build heatmaps of activity across different times and departments (Fire, EMS, Traffic).

> ✅ Ideal for showcasing data wrangling, feature engineering, and data visualization skills.

---

## 📈 Key Features

- 📌 Exploratory Data Analysis (EDA)
- ⏰ Time-based trend extraction (hour, day, month, year)
- 🧠 Feature Engineering (extracting reason, zip trends, time features)
- 📊 Visualizations (bar plots, line plots, heatmaps, clustermaps)
- 🌐 Geographic call frequency by zip code and township

---

## 🗂️ Dataset Information

- **Source**: [Kaggle - Montgomery County 911 Calls](https://www.kaggle.com/datasets/mchirico/montcoalert)
- **File**: `911.csv`
- **Size**: ~175K records
- **Features**:
  - `lat`, `lng`: Geolocation
  - `desc`: Call description
  - `zip`, `twp`: Zip code and township
  - `title`: Emergency type
  - `timeStamp`: Timestamp of the call
  - `e`: Emergency code

---

## 🛠️ Technologies & Libraries

| Language/Tool | Use |
|---------------|-----|
| **Python 3**  | Programming language |
| **Pandas**    | Data manipulation |
| **NumPy**     | Numerical operations |
| **Matplotlib**| Data visualization |
| **Seaborn**   | Advanced plotting |
| **Jupyter Notebook** | Development environment |

---

## 📊 Sample Insights & Visuals

Here are some of the analyses performed:

- **Top Emergency Types**:
  - EMS (Medical)
  - Fire
  - Traffic

- **Trends Discovered**:
  - Most calls happen during the day, especially around 5 PM.
  - EMS-related calls are the most frequent.
  - Certain zip codes dominate the call volume.

- **Visual Outputs**:
  - 🔵 Count plots for emergency types
  - 🔥 Heatmaps of day/hour call frequency
  - 📈 Time series line plots for daily calls
  - 🗓️ Monthly and yearly trends

---

## ▶️ How to Run the Project

1. **Clone the repository** or download the files:
   ```bash
   git clone https://github.com/yourusername/911-calls-analysis.git
   cd 911-calls-analysis
   ```
2. **Install dependencies**:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
3. **Launch the notebook**:
   ```bash
   jupyter notebook "01-911 Calls Data Capstone Project.ipynb"
   ```
## 📘 Folder Structure
📁 911-Calls-Dat_Analysis/

├── 📄 01-911 Calls Data Capstone Project.ipynb

├── 📄 911.csv

└── 📄 README.md

## 🎯 Learning Outcomes
1. Efficiently handled time-series data using datetime

2. Created multiple features from raw data

3. Built rich visualizations using seaborn and matplotlib

4. Gained actionable insights from real emergency call logs

## 🔖 Future Enhancements
1. Add geospatial visualizations using folium or plotly

2. Build a predictive model to forecast emergency call volume

3. Integrate interactive dashboards using Streamlit

## 📬 Contact
Author: Yash Upadhyay
📧 Email: yashupadhyay481@gmail.com
🔗 [LinkedIn](www.linkedin.com/in/yash-upadhyay-309b44281) | [GitHub](https://github.com/yash6810)
