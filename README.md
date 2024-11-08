# Deaths-in-US

Certainly! Here's a sample README for your GitHub repository based on the content provided:

---

# Exploratory Data Analysis on Deaths in the US (2005-2015)

## Introduction
This repository contains an exploratory data analysis (EDA) on the deaths dataset from the United States, spanning multiple years (2005-2015). The dataset consists of various attributes such as resident status, age, race, education, and causes of death. The goal of this analysis is to provide insights into trends, correlations, and distributions based on the data.

## Dataset Overview
The dataset includes several CSV files with data from different years:

- `2005_data.csv`
- `2006_data.csv`
- `2007_data.csv`
- `2008_data.csv`
- `2009_data.csv`
- `2010_data.csv`
- `2011_data.csv`
- `2012_data.csv`
- `2013_data.csv`
- `2014_data.csv`
- `2015_data.csv`

Each file contains the following key information:
- Resident status
- Education (1989 and 2003 revisions)
- Sex
- Age details
- Race and ethnicity data
- Cause of death
- Various flags and conditions related to the data

## Getting Started

To get started, simply clone this repository and open the Jupyter Notebook file `SQL_DeathInUS.ipynb`. Make sure to install the required dependencies.

### Requirements
- Python 3.x
- Libraries:
  - pandas
  - numpy
  - matplotlib
  - sklearn
  - seaborn
  - os

You can install these dependencies using `pip`:
```bash
pip install pandas numpy matplotlib scikit-learn seaborn
```

### File Structure
```
/ (root)
│
├── SQL_DeathInUS.ipynb    # Jupyter Notebook for data analysis
├── 2005_data.csv          # Data from the year 2005
├── 2006_data.csv          # Data from the year 2006
├── 2007_data.csv          # Data from the year 2007
├── ...
└── 2015_data.csv          # Data from the year 2015
```

## Analysis

The analysis in this repository is focused on understanding the distribution of data and exploring relationships between different features. The following plots are generated for each year's dataset:

1. **Distribution Graphs (Histograms/Bar Graphs)**: These plots show the distribution of sampled columns to understand the frequency of different values within them.
2. **Correlation Matrix**: A matrix displaying the correlation between different numerical features in the dataset.
3. **Scatter and Density Plots**: A scatter matrix is used to visualize pairwise relationships and kernel density estimation for numerical features.

### Example Code Snippets
Here's an example of how to read the data and plot the distributions:

```python
import pandas as pd
import matplotlib.pyplot as plt

# Read the data
df1 = pd.read_csv('2005_data.csv', nrows=1000)

# Plot distribution of columns
plotPerColumnDistribution(df1, 10, 5)

# Plot correlation matrix
plotCorrelationMatrix(df1, 8)

# Scatter matrix
plotScatterMatrix(df1, 20, 10)
```

## Conclusion
This repository provides a foundation for performing exploratory data analysis on a complex dataset of deaths in the US. It includes visualizations that can help in identifying patterns, trends, and correlations within the data. Feel free to modify and extend the analysis to suit your needs.

## License
This project is open-source and available under the MIT License.

---
