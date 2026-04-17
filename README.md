# 📊 Data Analytics Project

> End-to-end data analytics pipeline — from raw data to interactive dashboard and executive presentation.

---

## 📌 Overview

This project demonstrates a complete data analytics workflow, covering data ingestion, exploratory data analysis (EDA), data cleaning, SQL-based querying, business intelligence dashboarding, and stakeholder reporting. It is designed to reflect real-world analyst responsibilities across the full data lifecycle.

**Business Goal:** Uncover actionable insights from the dataset to support data-driven decision-making.

---

## 📁 Dataset

| Property       | Details                          |
|----------------|----------------------------------|
| **Source**     | [Add source — Kaggle / internal / API] |
| **Format**     | CSV / Excel / JSON               |
| **Size**       | [e.g., 50,000 rows × 12 columns] |
| **Key Fields** | [e.g., Date, Region, Sales, Category, Customer ID] |

> 📂 Dataset is stored in the `/data` folder. Raw data is kept in `/data/raw/` and cleaned data in `/data/processed/`.

---

## 🛠️ Tools & Technologies

| Layer              | Tool / Technology                          |
|--------------------|--------------------------------------------|
| **Language**       | Python 3.x                                 |
| **Data Wrangling** | Pandas, NumPy                              |
| **Visualization**  | Matplotlib, Seaborn                        |
| **Database**       | PostgreSQL / MySQL / SQL Server            |
| **BI Dashboard**   | Power BI Desktop                           |
| **Reporting**      | PDF / Word Report                          |
| **Presentation**   | Gamma (AI-powered PPT)                     |
| **Notebook**       | Jupyter Notebook                           |
| **Version Control**| Git & GitHub                               |

---

## 🔢 Project Steps

### 1. 🐍 Data Loading (Python)
- Imported the dataset using **Pandas** (`pd.read_csv()` / `pd.read_excel()`)
- Previewed structure with `.head()`, `.info()`, `.describe()`
- Identified data types, column names, and initial anomalies

**File:** `notebooks/01_data_loading.ipynb`

---

### 2. 🔍 Exploratory Data Analysis (EDA)
- Analyzed distributions, trends, and correlations
- Generated visualizations: histograms, bar charts, heatmaps, box plots
- Identified key patterns and business-relevant insights
- Detected outliers and missing values

**File:** `notebooks/02_eda.ipynb`

---

### 3. 🧹 Data Cleaning
- Handled missing values (imputation / removal)
- Removed duplicate records
- Standardized column names and data types
- Treated outliers using IQR method
- Exported cleaned dataset to `/data/processed/`

**File:** `notebooks/03_data_cleaning.ipynb`

---

### 4. 🗄️ SQL Queries (PostgreSQL / MySQL / SQL Server)
- Loaded cleaned data into the database
- Wrote SQL queries to answer key business questions:
  - Revenue by region and product category
  - Month-over-month growth trends
  - Top-performing segments and customer cohorts
  - Aggregations, window functions, and subqueries

**File:** `sql/queries.sql`

---

### 5. 📊 Power BI Dashboard
- Connected Power BI to the database / cleaned CSV
- Built interactive visuals: KPI cards, bar/line charts, slicers, maps
- Applied DAX measures for calculated metrics (e.g., YTD Sales, Growth %)
- Designed a clean, executive-ready layout with drill-through filters

**File:** `dashboard/dashboard.pbix`

> 📸 Screenshots available in `/dashboard/screenshots/`

---

### 6. 📝 Report
- Summarized methodology, findings, and recommendations
- Written for a non-technical stakeholder audience
- Includes charts exported from Python and Power BI

**File:** `report/analytics_report.pdf`

---

### 7. 📽️ Presentation (Gamma)
- Created a concise executive presentation using **Gamma**
- Covers: problem statement, key insights, dashboard walkthrough, recommendations
- Exported as PDF/PPT for sharing

**File:** `presentation/analytics_presentation.pdf`

---

## 📈 Dashboard Preview

> *(Add a screenshot of your Power BI dashboard here)*

```
dashboard/screenshots/dashboard_overview.png
```

---

## 💡 Key Results & Insights

> *(Replace with your actual findings once analysis is complete)*

- 📌 **Insight 1:** [e.g., Region X accounted for 42% of total revenue in Q3]
- 📌 **Insight 2:** [e.g., Customer churn increased by 15% in the last two quarters]
- 📌 **Insight 3:** [e.g., Product category Y showed the highest month-over-month growth at 23%]
- 📌 **Recommendation:** [e.g., Prioritize retention efforts in Region Z based on declining order frequency]

---

## 🗂️ Project Structure

```
📦 data-analytics-project/
├── 📁 data/
│   ├── raw/                  # Original, unmodified dataset
│   └── processed/            # Cleaned and transformed data
├── 📁 notebooks/
│   ├── 01_data_loading.ipynb
│   ├── 02_eda.ipynb
│   └── 03_data_cleaning.ipynb
├── 📁 sql/
│   └── queries.sql
├── 📁 dashboard/
│   ├── dashboard.pbix
│   └── screenshots/
├── 📁 report/
│   └── analytics_report.pdf
├── 📁 presentation/
│   └── analytics_presentation.pdf
├── requirements.txt
└── README.md
```

---

## ▶️ How to Run

### Prerequisites
- Python 3.8+
- Jupyter Notebook or JupyterLab
- PostgreSQL / MySQL / SQL Server (with a database set up)
- Power BI Desktop (Windows)

### Setup

```bash
# 1. Clone the repository
git clone https://github.com/your-username/data-analytics-project.git
cd data-analytics-project

# 2. Install Python dependencies
pip install -r requirements.txt

# 3. Launch Jupyter Notebook
jupyter notebook
```

### Run the Notebooks (in order)
```
1. notebooks/01_data_loading.ipynb
2. notebooks/02_eda.ipynb
3. notebooks/03_data_cleaning.ipynb
```

### Run SQL Queries
```sql
-- Connect to your database, then run:
\i sql/queries.sql        -- PostgreSQL
SOURCE sql/queries.sql;   -- MySQL
-- Or paste queries directly in SQL Server Management Studio (SSMS)
```

### Open Power BI Dashboard
```
Open Power BI Desktop → File → Open → dashboard/dashboard.pbix
Refresh data source connection if needed.
```

---

## 📦 Requirements

```
pandas
numpy
matplotlib
seaborn
jupyter
sqlalchemy
psycopg2-binary       # For PostgreSQL
pymysql               # For MySQL
pyodbc                # For SQL Server
```

> Full list in `requirements.txt`

---

## 👤 Author

**Jason**
📧 [your.email@example.com]
🔗 [LinkedIn Profile](https://linkedin.com/in/your-profile)
🐙 [GitHub](https://github.com/your-username)

---

## 📄 License

This project is licensed under the MIT License. See `LICENSE` for details.
