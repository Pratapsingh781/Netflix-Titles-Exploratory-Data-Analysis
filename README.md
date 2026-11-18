# Netflix Titles — Exploratory Data Analysis

## Project overview
This project performs exploratory data analysis on the cleaned Netflix titles dataset (`netflix_titles_cleaned.csv`) using Python.

## Files
- `Netflix_Titles_EDA.ipynb` — complete EDA notebook with code, statistics and visualizations.
- `netflix_titles_cleaned.csv` — dataset used by the notebook.

## How to run
1. Download or clone this repository.
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
3. Start Jupyter:
   ```bash
   jupyter notebook
   ```
4. Open `Netflix_Titles_EDA.ipynb` and run all cells.

## Main analysis
- Dataset structure and descriptive statistics
- Missing values and duplicate checks
- Movie vs TV Show distribution
- Release-year and Netflix-addition trends
- Content ratings and country-field distribution
- Movie runtime and TV season analysis
- IQR-based candidate outlier check

## Key findings
- 8,807 records and 15 columns.
- 6,131 Movies (69.6%) and 2,676 TV Shows (30.4%).
- No duplicate rows detected.
- 10 records have missing `date_added`, `year_added` and `month_added` values.
- The most frequent release year is 2018 (1,147 titles).
- The most frequent rating is TV-MA (3,207 titles).
- Median movie duration is 98 minutes.
- Median TV Show length is 1 season.
- The highest number of additions in the dataset occurred in 2019 (2,016 titles).

## Notes
Country values may contain multiple countries in one cell. The country chart counts the raw field values, excluding `Unknown`; it does not split co-productions. IQR outliers are candidates for review, not automatically errors.
