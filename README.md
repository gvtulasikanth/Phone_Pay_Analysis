**📊 PhonePe Pulse Data Analytics Project**
A complete end-to-end data pipeline, analysis, and dashboard visualization using Python, SQLite, and Power BI.

**📁 Project Overview**
This project extracts, transforms, and loads (ETL) data from the **PhonePe Pulse GitHub repository**, processes it into structured datasets, stores them in a **SQLite database**, and visualizes the insights through a **Power BI dashboard**.

**The project contains:**

dataextraction_checkpoint.py → Python script to scrape, clean, and store PhonePe Pulse data

Tulasikanth(phone pe project).pbix → Power BI dashboard for final data visualization

**🚀 Features**

**✔ Automated Data Extraction**

The Python script clones the official **PhonePe Pulse dataset**, then processes multiple categories:

Aggregated Transactions

Aggregated Insurance

Aggregated User Data

Map-based Transaction Data

Map-based Insurance Data

Map-based User Data

**✔ Data Transformation**

JSON files are parsed and converted into structured DataFrames using **Pandas**.

**✔ Centralized Database**

All processed data is inserted into a **SQLite database (pulse.db)** containing tables:

TRANSACTION_DATA

INSURANCE_DATA

USER_DATA

MAP_TRANSACTION

MAP_INSURANCE

MAP_USER

**✔ Data Export**

Clean datasets are also exported as .csv files.

**✔ Power BI Dashboard**

The final dashboard visualizes:

Statewise & yearwise transactions

Insurance trends

User registrations & app opens

Heatmaps

District-level metrics

Growth patterns over years

**📂 Project Structure**

📦 PhonePe-Pulse-Analytics

├── dataextraction_checkpoint.py     # Python ETL script

├── Tulasikanth(phone pe project).pbix   # Power BI dashboard

├── pulse.db                         # SQLite DB (generated after running script)

├── agg_transaction.csv

├── agg_insurance.csv

├── agg_user.csv

├── map_transaction.csv

├── map_insurance.csv

└── map_user.csv

**🛠 Technologies Used**

**Python**	Data extraction, parsing, cleaning,
**Pandas**	Data transformation
**JSON**	Parsing raw PhonePe data
**SQLite**	Database storage
**Power BI**	Dashboard visualization
**Git**	Cloning PhonePe Pulse repository

**▶ How to Run the Script**

**1. Clone this repository:**
git clone <your-repo-url>
cd <your-repo-folder>

**2. Install dependencies:**
pip install pandas sqlite3 json

(SQLite & JSON come pre-installed with Python)

**3. Run the ETL script:**
python dataextraction_checkpoint.py

This will:

Clone the PhonePe Pulse dataset

Transform the data

Create pulse.db

Export all CSV files

**4. Open the Power BI dashboard:**

Open

Tulasikanth(phone pe project).pbix
in Power BI Desktop and connect it to the generated pulse.db.

**📊 Dashboard Insights**

The Power BI dashboard helps analyze:

**🔹 Digital transaction trends**

UPI growth across states

Transaction amounts and counts

Most active states and districts

**🔹 Insurance metrics**

Insurance adoption across regions

Year-wise insurance premium trends

**🔹 User engagement**

Registered users

App opens frequency

District-wise user distribution

**📌 Future Enhancements**

Add live data updates using GitHub API

Create an interactive web dashboard (Streamlit / Dash)

Integrate machine learning trend predictions

Deploy to cloud (AWS / Azure)
