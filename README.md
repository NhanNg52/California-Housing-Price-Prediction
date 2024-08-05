# California Housing Price Prediction

## Group Members
- Raphael Luis Santos
- Kelly Tran
- Rick Liu
- Huu Nhan Nguyen
- Amy Ionescu

## Abstract
This project explores the factors influencing California's high housing prices, focusing on ocean proximity and median income. Using Linear Regression, k-Nearest Neighbors (kNN), and Random Forest Regression, we identified significant positive correlations between housing prices, income, and proximity to the ocean. The findings highlight the challenges facing potential homeowners as the housing market continues to rise.

## Introduction
California's housing market is known for its high prices and ongoing crisis. This study analyzes historical data to answer:
1. How does ocean proximity affect housing values?
2. How does household income influence rising housing costs?
3. What can be inferred about current housing conditions?

We use data from the U.S. Census and various machine learning techniques to analyze and predict housing values, aiming to provide insights into the factors affecting housing affordability.

## Problem Definition
We investigate how different features impact housing prices across California using data analysis techniques. Specifically, we examine the effects of ocean proximity and household income on housing values, applying Linear Regression, kNN, and Random Forest Analysis.

## Data Exploration and Preprocessing
### Dataset Overview
The dataset, sourced from Kaggle, includes features such as:
- `longitude`: Longitude coordinate
- `latitude`: Latitude coordinate
- `housing_median_age`: Median age of housing units
- `total_rooms`: Total number of rooms
- `total_bedrooms`: Total number of bedrooms
- `population`: Total population
- `households`: Number of households
- `median_income`: Median income
- `median_house_value`: Target feature

### Data Exploration
- **Histograms and Box Plots**: Visualize feature distributions and identify outliers.
- **Correlation Heatmaps**: Show relationships between features and the target variable.
- **Scatter Plots**: Reveal trends and patterns related to geographic coordinates and housing values.

### Data Preprocessing
- **Handling Missing Data**: Ensured dataset integrity by removing or imputing missing values.
- **One-Hot Encoding**: Converted non-numeric features like 'ocean_proximity' to numerical values.
- **Feature Engineering**: Added `bedroom_ratio` and `household_rooms` for more nuanced insights.

## Models and Evaluation
### Linear Regression
- **Method**: Applied Linear Regression to predict housing prices.
- **Performance**: Achieved R-squared values around -0.623, indicating poor fit due to non-linear relationships.

### k-Nearest Neighbors (kNN)
- **Method**: Used kNN regression with varying numbers of neighbors (k) to predict housing values.
- **Performance**: Optimal k values were 10 and 12, yielding R-squared values of 0.77697 and 0.77613, respectively.

### Random Forest
- **Method**: Used Random Forest regression with multiple decision trees.
- **Performance**: Achieved an R-squared value of 0.8137, improving to 0.8258 with parameter tuning. Random Forest showed strong performance and indicated significant influence of median income on housing prices.

## Conclusion
The analysis reveals a significant positive correlation between ocean proximity and housing prices. However, the growing gap between median income and housing costs highlights affordability issues. These findings stress the need for targeted housing policies to address the challenges of homeownership in California.

## References
1. Cameron Nugent. 2023. California Housing Prices. Kaggle. Available at: [Kaggle Dataset](https://www.kaggle.com/datasets/camnugent/california-housing-prices)
2. U.S. Census Bureau. 1990. General Housing Characteristics, California. U.S. Department of Commerce. Available at: [Census Bureau](https://www2.census.gov/library/publications/decennial/1990/ch-1/ch-1-6.pdf)
3. Legislative Analyst’s Office. 2023. California’s High Housing Costs: Causes and Consequences. Available at: [LAO Report](https://lao.ca.gov/LAOEconTax/Article/Detail/793#:~:text=Affordability%20depends%20on%20both%20the,income%20in%202022%20(%2485%2C300).)
4. IBM. 2023. K-Nearest Neighbors (KNN). Available at: [IBM KNN](https://www.ibm.com/topics/knn#:~:text=The%20k%2Dnearest%20neighbors%20.)

## Task Distribution
- **Collecting and Preprocessing Data**: Huu Nhan Nguyen
- **Implementing & Evaluating Linear Regression**: Raphael Luis Santos
- **Implementing & Evaluating kNN**: Kelly Tran, Rick Liu
- **Implementing & Evaluating Random Forest**: Amy Ionescu
- **Algorithm Comparisons and Writing Report**: All

## Links
- **Submission Folder**: [Google Drive](https://drive.google.com/drive/folders/1d2HzqO9fKB5uTFTcvDhWQKH6MerqTmVz?usp=sharing)
- **Preprocessing and Linear Regression Code**: [Colab Notebook](https://colab.research.google.com/drive/1XAwoCqX-fDbs6Fv3m8cSb0KLDu485Yg1?usp=sharing)
- **kNN Code**: [Colab Notebook](https://colab.research.google.com/drive/1LSfKO-XFw9mzGHQMLMuvfY2Rk6hOmmDl?usp=sharing)
- **Random Forest Code**: [Colab Notebook](https://colab.research.google.com/drive/1Xz9SplK2dr2RcuBRzfr9A3UMSmOqZVRY?usp=sharing)
