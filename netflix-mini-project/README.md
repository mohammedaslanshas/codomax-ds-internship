# Netflix Content Analysis 🎬

A data analysis project exploring Netflix's content catalog (8,807 titles) to understand trends in content type, geography, genre, and audience ratings.

## Dataset
Source: [Netflix Movies and TV Shows - Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)
8,807 rows × 12 original columns (movies & TV shows metadata)

## Objectives
- Has Netflix's content mix shifted between Movies and TV Shows over time?
- Which countries produce the most Netflix content?
- What are the most common genres?
- How does content rating vary between Movies and TV Shows?

## Process
1. **Data Cleaning** — handled missing values (fill vs drop based on severity), converted `date_added` to datetime, engineered `year_added`/`month_added`, split ambiguous `duration` column into number + unit
2. **Exploratory Data Analysis** — used groupby, crosstab, and `.explode()` to analyze multi-value genre data
3. **Visualization** — line charts, bar charts, and stacked bar charts using Matplotlib/Seaborn

## Key Insights
- Movies dominate in raw volume every year, but TV Shows' *share* of new content grew from 0% (2009-2012) to a stable ~29-34% (2017-2021) — a genuine long-term shift in content mix, even though Movies still lead overall
- The US and India are the top content-producing countries, though a notable share of country data was missing and filled as "Unknown"
- International Movies, Dramas, and Comedies are the top 3 genres
- TV-MA and TV-14 are the most common ratings, showing Netflix's catalog skews toward mature/teen audiences over children's content

## Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Google Colab

## Author
Mohammed Aslansha S — Data Science Intern @ Codomax Digital Solutions
