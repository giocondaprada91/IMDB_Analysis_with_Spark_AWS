# Analyzing IMDB Datasets

## Overview
This project involves analyzing IMDB datasets sourced from Kaggle to answer business questions about movies, genres, job categories, and actors using **Apache Spark** on AWS EMR. The analysis was performed using a Jupyter Notebook, and the outputs are consolidated in the `Project_Analysis.ipynb` file.

---

## Project Objectives
1. **Provision a Spark Cluster**: Set up an AWS EMR cluster to process large datasets.
2. **Analyze Data**: Use PySpark transformations and actions to answer analytical questions.
3. **Demonstrate Skills**: Showcase proficiency in data analysis and infrastructure setup using cloud technologies.

---

## Project Structure
```
Analyzing_IMDB_Datasets/
├── Project_Analysis.ipynb          # Jupyter Notebook with all analysis and code outputs
├── Project_Analysis.pdf            # PDF version of the notebook
└── README.md                       # Project description and usage instructions
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

## Technologies Used
- **Apache Spark**: For distributed data processing.
- **AWS EMR**: To provision a Spark cluster and handle computations.
- **Python Libraries**: `pandas`, `matplotlib`, `pyspark`.
- **Jupyter Notebook**: For interactive analysis and visualization.

---

## How to Reproduce
1. Clone this repository:
   ```bash
   git clone https://github.com/giocondaprada91/Analyzing_IMDB_Datasets.git
   ```
2. Set up an AWS EMR cluster and connect it to Jupyter Notebook.
3. Update the S3 bucket paths in the `Project_Analysis.ipynb` file to access the datasets.
4. Execute the notebook to reproduce the results.

---

## Submission Artifacts
- **Jupyter Notebook (`Project_Analysis.ipynb`)**: Contains all analysis and outputs.
- **PDF (`Project_Analysis.pdf`)**: Exported version of the notebook.
- **README (`README.md`)**: This file describing the project and its components.

---

## Acknowledgment
This project was completed as part of the Data Mining for Business Analytics course at Baruch College. The datasets were sourced from Kaggle and analyzed using AWS EMR and PySpark.
