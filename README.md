# Netflix-films-EDA-analysis
# Netflix Originals – Exploratory Data Analysis (EDA)

## Project Overview

This project focuses on performing Exploratory Data Analysis (EDA) on the Netflix Originals dataset using Python. The main objective is to explore movie characteristics, identify patterns and trends, and extract meaningful insights through statistical analysis and data visualization.

The analysis covers various aspects of Netflix Originals, including movie genres, languages, release dates, runtimes, and IMDb ratings.

## Dataset Description

The dataset contains **584 Netflix Original movies** and 6 features:

| Column | Description |
|---|---|
| `Title` | Movie title |
| `Genre` | Movie genre |
| `Premiere` | Original release date |
| `Runtime` | Movie duration in minutes |
| `IMDB Score` | IMDb rating |
| `Language` | Original language(s) of the movie |

## Project Objectives & Key Questions

The analysis addresses the following 15 questions:

1. Which languages are most common among long-running movies (120+ minutes)?
2. What are the IMDb ratings of Documentary movies released between January 2019 and June 2020?
3. Which genre has the highest average IMDb rating among English-language movies?
4. What is the average runtime of Hindi-language movies?
5. How many unique genres are represented in the dataset?
6. What are the three most frequently used languages?
7. Which 10 movies have the highest IMDb ratings?
8. Is there a correlation between movie runtime and IMDb scores?
9. Which 10 genres have the highest average IMDb ratings?
10. Which 10 movies have the longest runtimes?
11. In which year were the most movies released?
12. Which languages have the lowest average IMDb ratings?
13. Which year has the highest total movie runtime?
14. What is the most common genre for each language?
15. Are there any outliers in the dataset?

## Methodology

The project follows a structured EDA workflow:

**1. Data Exploration**
- Examining dataset structure, dimensions, and data types.
- Generating descriptive statistics.
- Identifying missing values and duplicate records.

**2. Data Cleaning & Preprocessing**
- Handling missing and duplicate values.
- Converting release dates into datetime format.
- Converting numerical columns into appropriate data types.
- Extracting release years from premiere dates.
- Splitting multiple languages into individual categories using `str.split()` and `explode()`.

**3. Exploratory Data Analysis**
- Univariate analysis of genres, languages, runtimes, and IMDb ratings.
- Comparative analysis across different languages and genres.
- Time-based analysis of movie releases and runtimes.
- Correlation analysis between numerical variables.
- Outlier detection using the Interquartile Range (IQR) method.

**4. Data Visualization**
- Bar plots for categorical comparisons.
- Histograms and KDE plots for distribution analysis.
- Scatter plots and regression lines for correlation analysis.
- Heatmaps for correlation visualization.
- Box plots for outlier detection.

## Tools & Technologies

- **Python** – Main programming language
- **Pandas** – Data manipulation and analysis
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Google Colab / Jupyter Notebook** – Development environment

## Key Analytical Considerations

- Movies with multiple languages (e.g., `English/Japanese`) are separated into individual language categories to ensure each language is included in the analysis.
- Long-running movies are defined as films with a runtime of **120 minutes or more** for this project.
- A minimum of 5 movies is used when comparing average IMDb ratings across genres and languages to reduce the influence of categories with very small sample sizes.
- Outliers are identified using the IQR method. They are not automatically removed, as unusually high or low values may represent valid movie characteristics.

## Repository Structure

```text
Netflix-Originals-EDA/
│
├── Netflix_Originals_EDA.ipynb
├── NetflixOriginals.csv
└── README.md
```

## How to Run the Project

1. Clone this repository:

   ```bash
   git clone https://github.com/YOUR-USERNAME/Netflix-Originals-EDA.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Netflix-Originals-EDA
   ```

3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

4. Open the notebook using Jupyter Notebook or upload it to Google Colab.

5. Load the dataset and run the notebook cells sequentially to reproduce the analysis and visualizations.

## Conclusion

This project demonstrates practical applications of Python-based Exploratory Data Analysis, including data cleaning, preprocessing, statistical analysis, and visualization.

It provides an opportunity to explore relationships between movie characteristics and IMDb ratings while developing a better understanding of the dataset through data-driven insights.

---

**Project Type:** Exploratory Data Analysis (EDA)  
**Domain:** Movies & Entertainment  
