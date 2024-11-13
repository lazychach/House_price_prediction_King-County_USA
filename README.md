# House Price Prediction in King County, USA

This project leverages **data analysis** and **machine learning** to predict house sale prices in King County, including Seattle, using data from sales recorded between **May 2014 and May 2015**. The main objective is to model the relationship between property features (such as area, location, number of bedrooms) and sale prices, using a **linear regression model** built with **PySpark**.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Project Workflow](#project-workflow)
- [Results](#results)
- [Future Improvements](#future-improvements)
- [Contributors](#contributors)

---

## Project Overview

Real estate prices vary widely depending on location, property characteristics, and market conditions. This project aims to create a predictive model that can estimate home prices in King County. The approach involves:
1. Data loading and preparation
2. Exploratory data analysis
3. Model training and evaluation using linear regression
4. Results visualization and interpretation

## Dataset

The dataset is sourced from [Kaggle](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction) and contains 21,600 records on home sales in King County, covering key features including:
- `id` : unique ID for each sale
- `date` : date of sale
- `price` : sale price (target variable)
- `bedrooms`, `bathrooms`, `sqft_living`, `sqft_lot` : property characteristics
- `floors`, `waterfront`, `view`, `condition`, `grade` : property quality indicators
- `yr_built`, `yr_renovated` : construction/renovation year
- `zipcode`, `lat`, `long` : location information
- and more…

## Installation

To get started, ensure you have the following installed:
- **Python 3.8+**
- **Apache Spark** with PySpark (instructions [here](https://spark.apache.org/docs/latest/api/python/getting_started/index.html))
- **Plotly** for visualization (optional but recommended)

Clone this repository and install dependencies:
```bash
git clone https://github.com/lazychach/house-price-prediction.git
cd house-price-prediction
pip install -r requirements.txt
```

## Project Workflow

1. **Data Loading and Preparation**:
   - Import the dataset with PySpark.
   - Handle missing values, duplicates, and apply normalization.
  
2. **Exploratory Data Analysis**:
   - Calculate descriptive statistics and visualize key features.
   - Use scatter plots, histograms, and correlation matrices to understand variable relationships.
  
3. **Predictive Modeling**:
   - Split the dataset into training and testing sets (80/20 split).
   - Train a linear regression model using PySpark MLlib.
   - Evaluate the model using **Mean Squared Error (MSE)** and **Mean Absolute Error (MAE)**.
  
4. **Results Visualization**:
   - Compare actual and predicted prices in a scatter plot to assess model accuracy.
   - Present insights gained from the model predictions.

## Results

The trained model provides insights into the key factors influencing house prices in King County. By understanding the correlation between features and sale prices, this project can support data-driven decisions in real estate investments.

## Future Improvements

- **Feature Engineering**: Add more location-based features or interactions.
- **Model Optimization**: Experiment with different regression techniques or ensemble models.
- **Scalability**: Extend the analysis to larger datasets or real-time data with Spark Streaming.

## Contributors

- [LazyChach](https://github.com/lazychach)
