#  Disney+ Movies Analysis

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-yellow)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-red)

##  Project Overview

This project performs **Exploratory Data Analysis (EDA)** on a dataset
of **Disney+ movies and shows** to uncover patterns in **ratings,
genres, directors, and release trends**.

The goal of this project is to:

-   Clean and preprocess movie datasets
-   Perform data exploration
-   Generate visual insights
-   Understand content trends on Disney+

This project demonstrates **data analysis skills using Python and
visualization libraries**.

------------------------------------------------------------------------

#  Project Structure

disney-plus-movie-analysis │ ├── movieanalysis.ipynb \# Main analysis
notebook ├── disney_plus_shows.csv \# Dataset └── README.md \# Project
documentation

------------------------------------------------------------------------

# 🛠️ Tech Stack

  Tool               Purpose
  ------------------ ------------------------------
  Python             Programming
  Pandas             Data cleaning & manipulation
  NumPy              Numerical operations
  Matplotlib         Data visualization
  Seaborn            Statistical visualization
  Jupyter Notebook   Interactive analysis

------------------------------------------------------------------------

# Dataset Description

The dataset contains information about **Disney+ titles**, including:

  Column         Description
  -------------- -----------------------
  Title          Movie/Show name
  Director       Director of the title
  Genre          Genre categories
  IMDb Rating    IMDb score
  Release Year   Year of release
  Language       Language of the title
  Country        Country of production
  Actors         Main cast
  Plot           Short description

------------------------------------------------------------------------

#  Data Preprocessing

Key data cleaning steps:

-   Handling missing values
-   Dropping incomplete records
-   Cleaning release year values
-   Splitting genre lists
-   Exploding genres for analysis

Example:

``` python
dataframe.dropna(
    subset=['imdb_rating','released_at','language','country','actors','plot'],
    inplace=True
)
```

------------------------------------------------------------------------

# Exploratory Data Analysis

The notebook explores several insights:

### Missing Value Analysis

Understanding missing data distribution across columns.

### Movie Release Trends

Analyzing how Disney+ content has evolved over time.

### Top Directors

Identifying directors with the most titles on the platform.

### Genre Analysis

Exploring which genres have higher IMDb ratings.

Example analysis:

``` python
genre_rating = df_exploded.groupby('genre_list')['imdb_rating'].mean()
```

------------------------------------------------------------------------

# 📊 Visualizations

The project includes several visualizations:

-   Bar Charts
-   Line Plots
-   Missing Data Charts
-   Genre vs Rating Comparisons

Libraries used:

-   Matplotlib
-   Seaborn

------------------------------------------------------------------------

#  How to Run the Project

### Clone the Repository

git clone https://github.com/yourusername/disney-plus-movie-analysis.git

###  Install Dependencies

pip install pandas numpy matplotlib seaborn jupyter

###  Run the Notebook

jupyter notebook movieanalysis.ipynb

------------------------------------------------------------------------

#  Key Insights

Some insights discovered:

✔ Certain genres consistently receive higher IMDb ratings\
✔ A small number of directors contribute many titles\
✔ Movie releases increased significantly in recent years

------------------------------------------------------------------------

#  Future Improvements

Possible next steps:

-   Build a movie recommendation system
-   Create a Power BI dashboard
-   Perform sentiment analysis on movie plots
-   Apply machine learning models for rating prediction

------------------------------------------------------------------------

#  Author

**Robin Ravichandran**

AI & Machine Learning Student\
Interested in Data Science \| AI \| Analytics

------------------------------------------------------------------------

 If you found this project useful, consider giving it a star on
GitHub.
