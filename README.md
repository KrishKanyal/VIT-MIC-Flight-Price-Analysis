# Flight Price Analysis & Visualization

## Project Overview
This repository contains a data science and visualization study analyzing flight pricing factors. Built for the Microsoft Innovations Club (MIC) AIML Department recruitment challenge (Track 3 - 1st Year Track).

## Problem Statement
Flight prices fluctuate dynamically based on multiple parameters, making it difficult for travelers to anticipate cost variations. This project cleans raw aviation data and generates key visual insights into price behaviors across airlines, booking windows, classes, and seasons.

## Dataset Used
- **Dataset Source:** Official dataset provided in the MIC recruitment challenge guidelines.
- **Cleaned Sample Count:** 41,898 records evaluated after missing value handling and duplicate removal.

## Methodology
1. **Data Ingestion:** Loaded raw CSV data using `pandas` DataFrames.
2. **Preprocessing & Cleaning:** Checked non-null counts, stripped missing entries with `dropna()`, and removed redundant rows with `drop_duplicates()`.
3. **Data Type Conversion:** Transformed price and timing metrics from string types to numeric formats (`pd.to_numeric`).
4. **Exploratory Data Analysis (EDA):** Engineered 5 core visualizations using `matplotlib` and `seaborn` to isolate key cost drivers.

## Technologies Used
- **Language:** Python
- **Environment:** Google Colab / Jupyter
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn

## Results & Key Findings
- **Travel Class Impact:** First Class and Business Class drive the highest average price tiers compared to Economy.
- **Booking Window Effect:** Prices decrease when booking well in advance (`Days_Before_Departure`), spiking significantly closer to departure date.
- **Airline Carrier Variance:** Premium carriers maintain consistently higher base prices than low-cost regional carriers.

## Challenges Faced
- **Data Format Inconsistencies:** Price columns contained string formats that required explicit type casting to numeric data prior to plotting.
- **Handling Missing Entries:** Mitigated null values safely without introducing distortion into average pricing metrics.

## Future Improvements
- Implement machine learning models (e.g., Random Forest Regression) to predict exact flight prices based on travel inputs.
- Build an interactive Streamlit or Gradio dashboard for live price exploration.

## Installation & Setup Instructions
1. Clone this repository:
   ```bash
   git clone [https://github.com/KrishKanyal/VIT-MIC-Flight-Price-Analysis.git](https://github.com/KrishKanyal/VIT-MIC-Flight-Price-Analysis.git)
