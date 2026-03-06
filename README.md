# Global Climate Dynamics: Clustering & Curve Fitting Analysis 🌍

## Project Overview
This project performs an advanced analytical study on the relationship between **Total Population growth** and **CO2 Emissions** using global World Bank datasets. By implementing K-Means Clustering and non-linear Curve Fitting, the suite identifies patterns in how different economies scale their carbon footprints relative to demographic shifts.

## Key Features
* **Automated Data ETL**: Custom filtering and cleaning of multi-year time-series data (2010–2019) from complex CSV structures.
* **K-Means Clustering Analysis**: Segments global data into distinct clusters to identify high-emission/low-population vs. high-population/efficiency-focused regimes.
* **Feature Normalization**: Implements data preprocessing and normalization to ensure unbiased clustering results.
* **Non-Linear Curve Fitting**: Utilizes Scipy's `curve_fit` to model the exponential relationship between population metrics and environmental impact.
* **Error Range Estimation**: Includes statistical functions for calculating upper and lower confidence limits for model predictions.

## Tech Stack
* **Language**: Python 3.x
* **Core Analytics**: Pandas, NumPy
* **Machine Learning**: Scikit-Learn (K-Means, Preprocessing)
* **Statistical Modeling**: SciPy (Curve Fitting, Optimization)
* **Visualization**: Matplotlib, Seaborn

## Analysis Workflow
1. **Correlation Assessment**: Uses Seaborn Pair Plots to visualize initial relationships between variables.
2. **K-Means Clustering**: Clusters data into 3 distinct operational zones based on CO2-to-Population ratios.
3. **Normalization**: Applies feature scaling to refine cluster centroids for higher accuracy.
4. **Exponential Modeling**: Fits an exponential growth function to project future CO2 trends based on population growth.

## How to Run
1. Ensure `population total.csv` and `co2 emmission.csv` are in the project directory.
2. Install dependencies: `pip install pandas numpy matplotlib seaborn scikit-learn scipy`
3. Execute the analysis: `python climate_clustering.py`
