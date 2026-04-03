# Retail Analytics Dashboard

**Marketing decision-support tool built with Streamlit - cohort analysis, RFM segmentation, customer lifetime value, and revenue forecasting.**

Analyzes e-commerce transaction data (Online Retail II dataset, 800K+ transactions) to help marketing teams understand customer behavior, identify high-value segments, simulate retention scenarios, and export actionable activation lists.

> **[Live Demo](https://retail-analytics-dashboard.streamlit.app)** (Streamlit Cloud)

---

## Pages

### KPIs Overview
Monthly and quarterly revenue trends, country breakdown, key business metrics at a glance.

### Cohort Analysis
Retention heatmaps by acquisition cohort - track how customer groups behave over time and identify when churn happens.

### RFM Segmentation
Segment customers by Recency, Frequency, and Monetary value. Identify Champions, At-Risk, Lost customers, and everything in between with interactive treemaps and distribution plots.

### Scenario Simulation
What-if analysis: simulate the revenue impact of improving retention by X%, increasing average order value, or reactivating dormant customers. Sensitivity analysis included.

### Advanced Analytics
Seasonality patterns, churn risk scoring, product affinity analysis, customer acquisition cost metrics, and revenue forecasting.

### Action Plan & Export
Generate activation lists filtered by segment, export CSVs ready for CRM or email campaigns. Executive summary auto-generation.

### Data Quality
Coverage report, missing value analysis, outlier detection - because insights are only as good as the data.

---

## Tech Stack

| Component | Technology |
|-----------|-----------|
| App framework | Streamlit |
| Data processing | Pandas, NumPy, SciPy |
| Visualization | Plotly, Matplotlib, Seaborn |
| Dataset | Online Retail II (UCI ML Repository) |

---

## Quick Start

```bash
git clone https://github.com/julesmortreux/retail-analytics.git
cd retail-analytics

pip install -r requirements.txt

streamlit run app/app.py
```

The app ships with a sample dataset (890 customers, 126K transactions). For the full dataset (5,939 customers, 800K transactions), download [Online Retail II](https://archive.ics.uci.edu/dataset/502/online+retail+ii) and place the cleaned CSV in `data/raw/`.

---

## Project Structure

```
retail-analytics/
├── app/
│   ├── app.py              # Main Streamlit app (7 pages, 2000+ lines)
│   └── utils.py            # Data processing, RFM, CLV, forecasting
├── notebooks/
│   └── Notebook.ipynb      # Data exploration & cleaning
├── data/
│   └── raw/                # Dataset (sample included)
├── experiments/
│   └── streamlit_v1.py     # Early prototype
└── requirements.txt
```

---

## Author

**Jules Mortreux** - Engineering student in Data & AI at ECE Paris.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jules-mortreux-960421292/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/julesmortreux)
