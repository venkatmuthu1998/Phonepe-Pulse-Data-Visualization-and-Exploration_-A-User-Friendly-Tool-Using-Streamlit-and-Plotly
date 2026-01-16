# 📊 PhonePe Data Visualization & Exploration

A Streamlit-based interactive dashboard for analyzing India’s PhonePe transaction ecosystem using aggregated, map, and top-level insights.


# 🚀 Project Overview

This project allows users to visually explore PhonePe’s transaction, insurance, and user-related datasets through:

Aggregated Analysis (Year-wise & quarter-wise)

Map-Level Analysis (State & District)

Top Statistics (Top/Bottom states, districts, brands, etc.)

The dashboard is fully interactive—sliders, dropdowns, and tabs dynamically generate charts using Plotly.


# 🧠 Features

1. Aggregated Analysis

Insurance, Transaction, and User data

Year-wise & quarter-wise analysis

State-level drilldowns

Transaction breakdown by type

Brand-wise mobile usage analytics

2. Map Analysis

Choropleth maps displaying state-level performance

District-level breakdown for each state

Registered users vs App opens trends

3. Top Charts

Quick insights:

Top mobile brands

Highest/lowest transaction states

Highest/lowest transaction districts

Top states by registered users

Top states by app opens

Top states by insurance transactions


# 🏗️ Project Architecture

Streamlit UI
│
├── Data Exploration
│   ├── Aggregated Analysis
│   ├── Map Analysis
│   └── Top Analysis
│
├── PostgreSQL Database
│   ├── aggregated_insurance
│   ├── aggregated_transaction
│   ├── aggregated_user
│   ├── map_insurance
│   ├── map_transaction
│   ├── map_user
│   ├── top_insurance
│   ├── top_transaction
│   └── top_user
│
└── Visualization Layer (Plotly)


# 🛢️ Data Source

Data is loaded from a PostgreSQL database (phonepe_data) using psycopg2.


# Tables used:

aggregated_insurance

aggregated_transaction

aggregated_user

map_insurance

map_transaction

map_user

top_insurance

top_transaction

top_user

# 🔧 Tech Stack

Python

Streamlit

Pandas

Plotly (Express & Graph Objects)

PostgreSQL

psycopg2

GeoJSON (India states)


# 📦 Installation & Setup

1. Clone the project
git clone https://github.com/yourusername/phonepe-streamlit-dashboard.git
cd phonepe-streamlit-dashboard

2. Install Dependencies
pip install -r requirements.txt

3. Setup PostgreSQL

Create a database:
CREATE DATABASE phonepe_data;
Import CSVs or use your dataset pipeline to load tables.


4. Update Database Credentials in code
Inside phonepe.py:
mydb = psycopg2.connect(
    host="localhost",
    user="postgres",
    password="your_password",
    database="phonepe_data",
    port="5432"
)

5. Run the Streamlit App
streamlit run phonepe.py



# 👤 Author

Venkatesan M

















