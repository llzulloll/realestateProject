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

## 📂 Project Structure

📂 Real Estate Investment Analysis
├── Real Estate Investing Report – Lorenzo Zullo.pdf   # Full project report
├── project.ipynb                                      # Code notebook
├── zillow-zhvi.csv                                    # Zillow housing index data
├── city_choropleth_map.html                           # Interactive investment map
└── city_heatmap.html                                  # Heatmap of top investment areas

## 🚀 How to Use
To view and interact with the analysis:
1. Clone this repository
2. Open `realestateProject/project.ipynb` in Jupyter Notebook or VS Code
3. Run all cells to generate predictions, scores, and visualizations
4. Open the generated `city_choropleth_map.html` and `city_heatmap.html` in your browser for interactive views

## 📈 Results
- **Top investment areas**: Florida, East Coast, parts of the Southwest
- **Best predictors**: ZHVI, bathroom count, and market growth
- **Challenges**: High price variability in luxury markets; future work may explore Random Forest or ensemble models.

## 🔭 Future Work
- Incorporate macroeconomic indicators (e.g. interest rates, job growth)
- Add neighborhood-level insights for better granularity
- Explore ensemble models to reduce high-value prediction error
