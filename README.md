🎯 1. Global Sales Tracker by Region

✅ Objective

Create a pipeline and dashboard that tracks global sales trends of Nintendo Switch games by region (North America, Europe, Japan, Others).


🛠️ Tech Stack

Area	Tool/Tech

Data Ingestion	Python (Requests, BeautifulSoup)

Orchestration	Airflow or Prefect

Storage	PostgreSQL (local or cloud)

Transformation	pandas or dbt (optional)

Visualization	Tableau / Power BI / Streamlit

Version Control	Git + GitHub

Documentation	Markdown (README, setup guide)

📁 GitHub Structure

pgsql

Copy

Edit

switch-sales-tracker/
├── data_ingestion/
│   └── vgchartz_scraper.py
├── airflow_dags/ OR prefect_flows/
│   └── sales_pipeline.py
├── database/
│   ├── schema.sql
│   └── seed_data/
├── notebooks/
│   ├── eda.ipynb
│   └── regional_trends.ipynb
├── dashboards/
│   └── Tableau_Public_Link.md
├── requirements.txt
├── README.md
└── .env (gitignored)


🗓️ Timeline: 4 Weeks

Week	Tasks

Week 1	Scrape/download VGChartz data by region, set up GitHub repo & PostgreSQL schema

Week 2	Build and schedule ETL pipeline with Airflow or Prefect

Week 3	Perform EDA: top genres/regions, moving averages, etc.

Week 4	Create Tableau/Power BI dashboard and document everything


🔧 Data Engineering (You)

Scrape or collect global Switch game sales from VGChartz (store region-wise data)

Build PostgreSQL schema: fact_sales, dim_game, dim_region

Orchestrate ETL pipelines (daily or weekly)

Ensure data quality: handle missing regions, misclassified genres

📊 Data Analysis (Friend)

Top-selling regions and genres

Trends over time (seasonality, spikes)

Insights like: “Europe favors RPGs more than NA”, etc.

Build dashboards with slicers by region, year, genre



🔄 Optional Extensions
Add price and revenue (if available)

Combine with Metacritic scores for deeper insights

Push cleaned data to a public REST API or Superset dashboard

