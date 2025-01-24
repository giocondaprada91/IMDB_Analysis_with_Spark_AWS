# Analyzing IMDB Datasets

## Overview
This project analyzes datasets related to movies, TV shows, actors, and ratings using **PySpark**, a distributed computing framework. It explores various questions and insights, including:

- Identifying the highest and lowest-rated movies in the Harry Potter franchise.
- Discovering movies featuring both Johnny Depp and Helena Bonham Carter.
- Determining the most engaged TV series featuring David Tennant.
- Exploring job categories and their prevalence in the dataset.

The project leverages powerful data manipulation capabilities to join, filter, and aggregate across multiple datasets to provide meaningful insights.

---

## Technologies Used
- **Apache Spark (PySpark)**: For distributed data processing, joining large datasets, and performing complex queries efficiently.
- **Python**: For scripting and additional analysis.
- **Matplotlib**: For generating visualizations of insights (e.g., top job categories).

---

## Data Sources
- **Name Basics (df1)**: Contains information about actors, actresses, and their professions.
- **Title Basics (df2)**: Includes metadata about movies and TV shows, such as titles, release years, and genres.
- **Title Principals (df3)**: Describes cast and crew details for each movie or show.
- **Title Ratings (df4)**: Provides average ratings and vote counts for titles.

---

## Project Structure
```
Analyzing_IMDB_Datasets/
├── Project_Analysis.ipynb          # Jupyter Notebook with all analysis and code outputs
├── Project_Analysis.pdf            # PDF version of the notebook
└── S3_Bucket_Data/                 # S3 bucket paths used in the analysis
```

---

## Analysis Components
### Part I: Installation and Initial Setup
- Installed necessary Python packages (`pandas`, `matplotlib`, `pyspark`).
- Loaded datasets from an S3 bucket into PySpark DataFrames.
- Provided an overview of dataset dimensions (rows and columns).

### Part II: Analyzing Movie Genres
- Denormalized genres and calculated:
  - Total unique genres.
  - Average rating per genre.
- Visualized the top genres using a horizontal bar chart.

### Part III: Analyzing Job Categories
- Extracted and analyzed job categories, including:
  - Total unique job categories.
  - Top job categories by frequency.
- Visualized top job categories using a bar chart.

### Part IV: Answering Analytical Questions
1. Movies released in 2023 with more than 50,000 votes and a rating of 8+.
2. Films featuring Cillian Murphy since 2007, including ratings and his highest-rated movie.
3. Zendaya's movie appearances by year.
4. Age at which Audrey Hepburn passed away.
5. Highest-rated movie featuring Chris Evans.
6. Comparison of average ratings between Clint Eastwood and Harrison Ford.
7. Movies featuring both Johnny Depp and Helena Bonham Carter.
8. Top TV series featuring David Tennant, ranked by viewer engagement.
9. Highest and lowest-rated movies in the Harry Potter franchise featuring Daniel Radcliffe.

---

## Reproducibility
### Environment Setup:
To replicate this analysis:
1. **Launch an AWS EMR Cluster**:
   - Configure an EMR cluster with Apache Spark and Jupyter Notebook enabled.
   - Use the EMR console to access the hosted Jupyter Notebook environment.

2. **Prepare Data**:
   - Upload the datasets to an S3 bucket and configure the cluster to access the data.
   - Load the datasets into Spark DataFrames (`df1`, `df2`, `df3`, `df4`).

3. **Run the Analysis**:
   - Execute the cells in `Project_Analysis.ipynb` to reproduce the results.

---

## Submission Artifacts
- **Jupyter Notebook (`Project_Analysis.ipynb`)**: Contains all analysis and outputs.
- **PDF (`Project_Analysis.pdf`)**: Exported version of the notebook.
- **README (`README.md`)**: This file describing the project and its components.

---

## Acknowledgment
This project was completed as part of the Data Mining for Business Analytics course at Baruch College. The datasets were sourced from Kaggle and analyzed using AWS EMR and PySpark.

