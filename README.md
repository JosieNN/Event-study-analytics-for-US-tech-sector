# Event-study-analytics-for-US-tech-sector
A scalable event-study analytics system for tracking market reactions to SEC filings in the technology sector. This project integrates structured financial data and unstructured filing text to enable large-scale empirical analysis.

---

## Overview

Traditional financial analytics platforms (e.g., Bloomberg) are expensive and limited in flexibility. This project provides an open and extensible alternative for conducting event-study analysis using publicly available data.

The system integrates:
- SEC EDGAR filings (10-K, 10-Q, 8-K)
- Market data from Yahoo Finance
- Hybrid database architecture (PostgreSQL + MongoDB)
- Event-study analytics (AR, CAR, volatility)

---

## Key Features

- End-to-end **ETL pipeline** for financial and filing data
- **Hybrid data storage**
  - PostgreSQL for structured financial data
  - MongoDB for unstructured SEC filing text
- Event-study analysis:
  - Abnormal Return (AR)
  - Cumulative Abnormal Return (CAR)
  - Volatility
- **Flask-based API and interactive dashboard**
- Scalable design for large-scale empirical research

---

## System Architecture

SEC EDGAR API + Yahoo Finance
→
ETL Pipeline
→
PostgreSQL (structured data) + MongoDB (filing text)
→
Event Study Engine
→
Flask API & Dashboard

---

## Tech Stack

- Programming: Python
- Data Processing: Pandas, NumPy
- Databases: PostgreSQL, MongoDB
- APIs: SEC EDGAR API, yfinance
- Backend: Flask

---

## Repository Structure

- notebooks/
  - event_study_pipeline.ipynb # Core ETL + analytics pipeline
- docs/
  - company_list.csv # US tech companies after cleaning
- requirements.txt
- .env.example
- README.md
