# SpaceX Falcon 9 First Stage Landing Prediction

This repository contains the final capstone project for the SpaceX Falcon 9 landing prediction problem.  
The goal is to explore historical launch data and build a classification model to predict whether the first stage will successfully land.

---

## Project Overview

**Objective:** Predict first-stage landing success (`Class`: 1 = success, 0 = failure) using launch/mission features.  
**Workflow:**
1. Data collection (SpaceX REST API + Wikipedia web scraping)
2. Data wrangling / cleaning and feature engineering
3. Exploratory Data Analysis (EDA) with visualization and SQL
4. Interactive analytics (Folium map + Plotly Dash dashboard)
5. Predictive modeling (classification) and evaluation

---

## Repository Structure

### Notebooks / Scripts
- **Collecting the data – API.ipynb**  
  SpaceX REST API calls and dataset construction.
- **Web scraping from Wikipedia.ipynb**  
  Scraping Falcon 9 launch records from Wikipedia tables.
- **Data wrangling.ipynb**  
  Data cleaning, filtering, handling missing values, and feature preparation.
- **EDA with Data Visualization.ipynb**  
  Visual EDA: relationships between success and features (payload, site, orbit, etc.).
- **EDA with SQL.ipynb**  
  SQL queries in SQLite to compute key aggregates and validate EDA insights.
- **Interactive Map with Folium.ipynb**  
  Launch sites map + outcomes + proximity distance analysis.
- **Dashboard with Plotly Dash.py**  
  Interactive dashboard (dropdown + slider + charts).
- **Predictive Analysis.ipynb**  
  Feature encoding/scaling + model training + GridSearchCV + evaluation.

---

## How to Run

### 1) Install dependencies
Recommended (minimal set):

```bash
pip install pandas numpy matplotlib seaborn scikit-learn plotly dash folium sqlalchemy
