# IMDB Movie Data Analysis Report

## Overview
This project is a standalone HTML report analyzing 1000 IMDB movies (2006–2016) to explore ratings, revenue, runtime, and genres. It features interactive visualizations (scatter plots, bar charts, line charts) and highlights that biographical films have high ratings despite lower revenue.

## Features
- **Dataset**: `IMDB-Movie-Data.csv` (1000 movies, columns: Rank, Title, Genre, etc.).
- **Analyses**:
  - Scatter plot: Rating vs. Revenue.
  - Bar chart: Average rating by genre.
  - Line chart: Runtime distribution.
- **Finding**: Biography genre has high ratings (~7.8) but lower revenue.

## Technologies
- **React**: Interactive UI.
- **Recharts**: Charts.
- **Tailwind CSS**: Styling (CDN).
- **PapaParse**: CSV parsing.
- **JavaScript**: Data processing.
- **HTML**: Report structure.

## Setup
1. **Open**: Run `movie-analysis-report.html` in a modern browser (e.g., Chrome).
2. **View**: Report loads with interactive charts and analysis.

**Note**: Assumes `loadFileData` provides CSV. If unavailable, host CSV or modify loading logic.

## Data Processing
- **Cleaning**: Converts numeric fields, splits genres, sets missing Revenue/Metascore to 0, discards invalid rows.
- **Aggregation**: Calculates average ratings by genre, bins runtimes (10-min intervals).

## Limitations
- Assumes `loadFileData` availability.
- Missing revenue data may skew results.
- Limited to 2006–2016.

## Future Improvements
- Add filters for years/genres.
- Analyze directors/actors.
- Support CSV uploads.

## License
For educational use. Ensure compliance with IMDB dataset terms.