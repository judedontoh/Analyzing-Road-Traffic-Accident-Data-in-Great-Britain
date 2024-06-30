# UK Road Accident Analysis

## Project Overview
This project analyzes road traffic accident data from Great Britain for the year 2020. The objective is to identify patterns and propose strategies to enhance road safety. The analysis includes data exploration, cleaning, visualization, statistical analysis, and predictive modeling.

## Motivation
Understanding the patterns and causes of road traffic accidents is critical for improving road safety. This project aims to leverage data analysis and machine learning techniques to uncover insights that can inform better safety measures and policies.

## Data Collection
The data includes records from four tables: accidents, vehicles, casualties, and LSOA for the year 2020. The dataset was sourced from the UK government’s open data portal.

## Code and Resources Used
- **Python Version**: 3.8
- **Packages**: pandas, matplotlib, seaborn, scikit-learn
- **Requirements**: `pip install -r requirements.txt`

## Data Exploration
```python
import pandas as pd

# Load the accident data
accidents = pd.read_csv('data/accident_data.csv')
```
### Data Cleaning
```python
from src.data_preprocessing import clean_data

# Clean the accident data
cleaned_accidents = clean_data(accidents)

```
## Data Visualization


### Plot the distribution of accidents
```python
plot_accidents(cleaned_accidents)
Statistical Analysis

from src.statistical_analysis import analyze_data
```
### Perform statistical analysis
```python
analysis_results = analyze_data(cleaned_accidents)
Predictive Modeling
from src.predictive_modeling import build_model

```
### Build and evaluate a predictive model
```python
model, evaluation = build_model(cleaned_accidents)
```
