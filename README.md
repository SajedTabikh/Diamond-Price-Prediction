# Diamond Price Analysis

## About the Dataset

This dataset contains the prices and other attributes of nearly 54,000 diamonds. There are 10 attributes in total, including the target variable, `price`.

### Attributes

- **carat**: The diamond’s physical weight measured in metric carats (0.2 - 5.01). One carat equals 0.20 grams.
- **cut**: The quality of the diamond's cut (Fair, Good, Very Good, Premium, Ideal).
- **color**: The diamond's color, ranging from J (worst) to D (best).
- **clarity**: The diamond's clarity, rated from I1 (worst) to IF (best).
- **depth**: The total depth percentage of the diamond, calculated as `z / mean(x, y)`.
- **table**: The width of the diamond's top relative to its widest point.
- **price**: The price of the diamond in US dollars (target variable).
- **x**: Length of the diamond (in mm).
- **y**: Width of the diamond (in mm).
- **z**: Depth of the diamond (in mm).

## Project Overview

This project involves the exploration, cleaning, and analysis of the diamond dataset. The goal is to understand the relationships between the diamond's features and its price.

### Libraries Used

- `numpy`
- `pandas`
- `statsmodels`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `xgboost`

### Data Cleaning

- Dropped the `Unnamed: 0` column.
- Converted categorical columns (`cut`, `color`, `clarity`) to the appropriate data types.

### Exploratory Data Analysis (EDA)

#### Distribution of Numerical Features

- Plotted the distribution of `price`, `carat`, and `table`.
- Applied log transformation to `price` and `carat` for normalization.
- Visualized the distributions of `x`, `y`, and `z` (length, width, depth).

#### Outliers Detection

- Used boxplots to identify outliers in `price`, `carat`, `table`, `x`, `y`, and `z`.

#### Relationships Between Numerical Features

- Created scatter plots of `log_price` vs `log_carat`, `depth`, `table`, `x`, `y`, and `z` to examine correlations.
- Generated a correlation heatmap to visualize the relationships between numerical features.

#### Categorical Features Analysis

- Created violin plots to visualize the distribution of `price` across different categories of `cut`, `color`, and `clarity`.
- Counted the occurrences of diamonds by `cut`, `color`, and `clarity`.

### Conclusion

This project provided a comprehensive analysis of the diamond dataset, exploring the relationships between various features and the diamond's price. The visualizations and analysis performed can help in understanding how different attributes of a diamond contribute to its market value.
