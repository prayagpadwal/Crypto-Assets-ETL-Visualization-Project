# Crypto Assets ETL & Visualization Project
![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Database-blue?logo=postgresql&logoColor=white)
![Apache Superset](https://img.shields.io/badge/Apache_Superset-Visualization-brightgreen?logo=apache&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-Reporting-success?logo=microsoft-excel&logoColor=white)
![ETL](https://img.shields.io/badge/ETL-Pipeline-yellowgreen?logo=apacheairflow&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-Data_Source-blue?logo=kaggle&logoColor=white)

## Overview
This project implements an end-to-end Extract, Transform, Load (ETL) pipeline designed for crypto asset data. It leverages Python for data extraction from various sources, PostgreSQL for storage, Apache Superset for visualization, and includes robust data modeling with technical indicators.

![diagram](https://github.com/user-attachments/assets/1d8d66dc-82f7-49f3-b4b2-0424bc1172da)


## Project Structure

### Data Flow
- **Data Sources**:
  - Kaggle API
  - Flat files (e.g., CSV)
- **ETL Pipeline**:
  - Data extraction and transformation handled via Python scripts.
  - Loaded into PostgreSQL database.
- **Data Modeling**:
  - Structured schema capturing crypto assets, price data, and computed technical indicators.
  - PostgreSQL relational database setup.
- **Reporting**:
  - Reports generated in Excel format for intermediate analysis.
- **Visualization**:
  - Interactive dashboards and reports created with Apache Superset.

## Database Schema
The PostgreSQL database schema includes:

- `crypto_assets`: Contains crypto asset details (ID, Name, Symbol).
- `price_data`: Contains historical price data (Timestamp, Open/Close Prices, Volume).
- `technical_indicators`: Computed metrics like volatility, moving averages, Bollinger bands, and more.
![drawio](https://github.com/user-attachments/assets/f27419f7-88a6-4d59-89cb-c49dcb71b8ff)

## Visualization Tool
Apache Superset is used for interactive data exploration and visualization, allowing intuitive insights into market trends and asset performance.

## Installation

### Requirements
- Python 3.x
- PostgreSQL
- Apache Superset

### Setup
1. Clone repository:
   ```bash
   git clone <repository-url>
   ```
2. Setup Python environment:
   ```bash
   pip install -r requirements.txt
   ```
3. Initialize PostgreSQL Database:
   ```sql
   CREATE DATABASE crypto_db;
   ```
4. Configure Apache Superset:
   Follow instructions on [Superset's official docs](https://superset.apache.org/docs/installation/installing-superset).

## Usage
- Run ETL scripts:
```bash
python etl.py
```
- Access Apache Superset:
```bash
superset run -p 8088
```
Navigate to `http://localhost:8088` to create and view dashboards.

## Contributing
Feel free to contribute by submitting pull requests. Ensure code is well-documented and tested.

## License
This project is licensed under the MIT License. See `LICENSE` for more details.

