# Crypto Assets ETL & Visualization Project

## Overview
This project implements an end-to-end Extract, Transform, Load (ETL) pipeline designed for crypto asset data. It leverages Python for data extraction from various sources, PostgreSQL for storage, Apache Superset for visualization, and includes robust data modeling with technical indicators.

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

