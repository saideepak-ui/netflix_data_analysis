📊 Netflix Data Cleaning, Analysis & Recommendation System
📌 Project Overview

This project focuses on cleaning, analyzing, visualizing, and building a simple recommendation model using the Netflix dataset.
The aim is to:

Explore Netflix’s catalog distribution (Movies vs TV Shows).

Identify popular genres, directors, and countries.

Study content release trends over time.

Build a content-based recommendation system in Python.

📂 Dataset

File: netflix1.csv

Size: ~7,800 rows

Columns:

show_id → Unique ID

type → Movie / TV Show

title → Content title

director, cast, country

date_added, release_year

rating, duration, listed_in (genres)

description

🛠️ Project Workflow
Phase 1: Data Cleaning

Removed duplicates.

Converted date_added into datetime.

Created new features:

year_added, month_added, day_added

Split listed_in into genres list

Parsed duration into duration_minutes (for Movies) and seasons (for TV Shows)

Filled missing values (e.g., director → "Not Given").

✅ Outcome: Clean dataset ready for analysis.

Phase 2: Exploratory Data Analysis (EDA)

Using Python (Matplotlib/Seaborn):

Content by Type → ~70% Movies, ~30% TV Shows.

Ratings Distribution → Most common: TV-MA, TV-14, TV-PG.

Top Countries → USA dominates, followed by India & UK.

Monthly Releases → Peaks around July–September.

Yearly Releases → Rapid growth from 2015, peak in 2019–2020.

Top Genres → Dramas, Comedies, International Movies.

Top Directors → Raúl Campos & Marcus Raboy lead.

✅ Outcome: Clear visualizations highlighting global content patterns.

Phase 3: Insights Summary

Netflix favors Movies over TV Shows.

Content growth accelerated in mid–2010s, peaking in 2019–2020.

Strong dominance of USA content, but India and UK are rising contributors.

Popular genres are Drama, Comedy, International.

Few directors contribute multiple titles.

Phase 4: ML — Content-Based Recommender

Built a recommendation system using:

TF-IDF Vectorization on genres

Cosine Similarity to measure closeness between shows/movies

Implemented recommend(title) function → suggests similar content.

Example: “Ganglands” → recommends other Action/Crime dramas.

✅ Outcome: Functional ML recommender integrated in Jupyter Notebook.

🚀 Tools & Libraries

Python → pandas, matplotlib, seaborn, scikit-learn

Jupyter Notebook → Cleaning, EDA, ML recommender

📌 Final Deliverables

Jupyter Notebook → Full project (cleaning + analysis + ML)

Visualizations → Content distribution, ratings, countries, genres, trends

Recommendation Engine → Suggests similar Netflix content
