# Real Estate Investment Analysis Tool 🏡📊  
**By Lorenzo Zullo** | Gettysburg College | DS 325 Final Project

## 📌 Overview
This project leverages **machine learning and geospatial data analysis** to identify high-opportunity real estate markets across the United States. By combining Zillow’s ZHVI index with detailed property listings, I built predictive models and created an **Investment Score** to rank cities by growth, affordability, and market volatility.

## 💡 Objectives
- Predict home prices using **Linear, Lasso, and Ridge Regression**
- Visualize growth and undervaluation trends using **heatmaps and choropleth maps**
- Rank cities using a custom **Investment Score** based on:
  - Price-to-ZHVI ratio
  - Market growth (2020–2025)
  - Price volatility

## 🧠 Methodology
- **Data Sources**:
  - [USA Real Estate Dataset](https://www.kaggle.com/datasets/ahmedshahriarsakib/usa-real-estate-dataset)
  - [Zillow Housing Index (ZHVI)](https://www.zillow.com/research/data/)
- **Tech Stack**: Python, Pandas, scikit-learn, Plotly, Folium, Geopy
- **Feature Engineering**: price/ZHVI ratio, growth rate, categorical encoding
- **Modeling**: Ridge regression performed best (R² ≈ 0.58), but struggled with outliers and luxury homes
- **Visualization**:
  - `city_choropleth_map.html`: Investment scores by city
  - `city_heatmap.html`: Top 100 high-opportunity locations

## 📁 Project Structure
