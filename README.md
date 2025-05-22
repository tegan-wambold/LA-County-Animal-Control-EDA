## 🐶 Animal Control Intake/Outcome Analysis

This project analyzes animal intake and outcome data from hte LA County Animal Care and Control system. It explores trends in animal adoptions, intake types, durations of stay, and more, using Python and data visualization libraries like `pandas`, `seaborn`, and `matplotlib`.

## Project Goals

- Understand outcome patterns (i.e. adoptions, euthanasia, etc.) by intake type, animal type, and seasonality
- Clean and preprocess data to correct inconsistent and missing data entries
- Visualize adoption rates and animal populations with clear, interpretable charts
 
### Files
- `Animal_Control_EDA.ipynb`: Exploratory data analysis
- `Data/Animal_Care_Pawstats.csv`: Dataset (source: [https://data.lacounty.gov/datasets/a02dbb13c2374a8985a471ee35d5923f_0/explore])

## Features & Methods

- **Data cleaning**: Handles missing values, converts dates, and corrects negative durations
- **Exploratory Data Analysis (EDA)**: Uses grouped bar plots, stacked bar plots, line graphs, histograms, and pivot tables
- **Custom metrics**: Calculates adoption proportions across categories
- **Visual storytelling**: Organizes multiple charts using `matplotlib` subplots

## Data Cleaning Highlights

- Ensures `Intake Date` and `Outcome Date` are valid datetime objects
- Detects and fixes rows where `Intake Date` is after `Outcome Date` by swapping values
- Recalculates `Duration (Days)` consistently after cleaning

### Requirements
- pandas
- matplotlib
- seaborn
- jupyter notebook

### How to Run
1. Clone the repo
2. Install dependencies
3. Run `Animal_Control_EDA.ipynb` in Jupyter

### Dataset
Downloaded from [https://data.lacounty.gov/datasets/a02dbb13c2374a8985a471ee35d5923f_0/explore].
