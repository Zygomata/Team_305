# 🎮 Nintendo Switch Global Sales Tracker

An end-to-end data engineering and data analysis project that collects, processes, and visualizes global Nintendo Switch game sales by region. Designed to enhance data engineering and data analysis skills through real-world, multi-source datasets and modern tooling.

---

## 🚀 Project Overview

This project tracks Nintendo Switch game sales across major regions (North America, Europe, Japan, Others) and provides insights into trends, top-performing genres, publishers, and regional preferences.

We use a modular pipeline to collect, clean, and load the data into a structured database, followed by exploratory analysis and interactive dashboards.

---

## 🛠️ Tech Stack

| Layer                | Tools / Libraries                             |
|---------------------|-----------------------------------------------|
| Data Ingestion       | `Python`, `Requests`, `BeautifulSoup`         |
| Workflow Orchestration | `Airflow` or `Prefect`                        |
| Data Storage         | `PostgreSQL` (Local or Cloud e.g. AWS RDS)    |
| Data Transformation  | `pandas`, optional: `dbt`                     |
| Data Analysis        | `Jupyter`, `seaborn`, `plotly`, `scikit-learn`|
| Visualization        | `Tableau`, `Power BI`, or `Streamlit`         |
| Version Control      | `Git`, `GitHub`                               |

---

## 📁 Repository Structure

```bash
switch-sales-tracker/
├── data_ingestion/
│   └── vgchartz_scraper.py             # Scrapes game sales by region
├── airflow_dags/ or prefect_flows/
│   └── sales_pipeline.py               # Scheduled ETL pipeline
├── database/
│   ├── schema.sql                      # SQL schema for PostgreSQL
│   └── seed_data/                      # Optional starter data
├── notebooks/
│   ├── eda.ipynb                       # Exploratory data analysis
│   └── regional_trends.ipynb          # Trend analysis per region
├── dashboards/
│   └── Tableau_Public_Link.md         # Link to live dashboard (if any)
├── requirements.txt                   # Project dependencies
├── .env                               # Credentials & DB URL (gitignored)
└── README.md                          # You are here 📍
````

---

## 🗓️ 4-Week Project Timeline

| Week   | Focus                                  | Deliverables                                 |
| ------ | -------------------------------------- | -------------------------------------------- |
| Week 1 | 📥 **Data Ingestion & Schema Design**  | Scraper script, SQL schema, source docs      |
| Week 2 | ⚙️ **ETL Pipeline Development**        | Prefect/Airflow flow, test loads, .env setup |
| Week 3 | 📊 **Exploratory Data Analysis (EDA)** | Jupyter notebooks, insights, graphs          |
| Week 4 | 📈 **Dashboard & Final Deliverables**  | Tableau dashboard, project report            |

---

## 🔧 Data Engineering Tasks (Arjun)

* ✅ Scrape global Switch game sales data from [VGChartz](https://www.vgchartz.com/gamedb/)
* ✅ Parse sales data by region (NA, EU, JP, Others)
* ✅ Design PostgreSQL schema:

  * `fact_sales`
  * `dim_games`
  * `dim_regions`
* ✅ Build an automated ETL pipeline using Prefect or Airflow
* ✅ Handle data quality issues (missing, duplicates, type mismatches)
* ✅ Enable downstream access via SQL views or REST API (optional)

---

## 📊 Data Analysis Tasks (Friend)

* 📈 Load cleaned data into notebooks for EDA
* 📊 Analyze:

  * Top-selling genres by region
  * Seasonal trends (monthly/quarterly sales)
  * Publisher performance across regions
* 📉 Identify patterns like:

  * Do RPGs perform better in Japan?
  * Are sports games more popular in North America?
* 📍 Build visual dashboards using Tableau, Power BI, or Streamlit
* 🧠 Optional: Build predictive models (e.g., top 10 game forecasts)

---

## 📌 Example Insights

* Which genres dominate in each global region?
* What time of year do sales spike most?
* Which publishers consistently produce best-selling games?
* How do regional trends change year over year?

---

## 📚 Data Sources

* 🎮 [VGChartz Game Sales Database](https://www.vgchartz.com/gamedb/)
* 🧾 Nintendo quarterly financial reports
* 🔍 (Optional) Metacritic or IGDB API for game metadata

---

## ✅ Final Deliverables

| Type             | Description                                         |
| ---------------- | --------------------------------------------------- |
| 📄 Documentation | `README.md`, schema, pipeline overview, usage guide |
| 💾 Database      | PostgreSQL with normalized schema and sample data   |
| 🧠 EDA Reports   | Jupyter notebooks with visual insights              |
| 📊 Dashboard     | Tableau/Power BI dashboard with filters/slicers     |
| 📂 Presentation  | Summary slides or executive report (optional)       |

---

## 🤝 Contributors

* **Arjun Gupta** – Data Engineering 
* **Dylan Roberts** – Data Analysis 

---

## 📄 License

[MIT License](LICENSE)

---
