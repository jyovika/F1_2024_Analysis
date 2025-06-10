# README — F1 Pit Stop Analysis

## Overview

This project investigates the impact of pit-stop speed on Formula 1 race outcomes across multiple seasons (2011, 2015, 2019, and 2024). Using publicly available data from the Ergast database, the analysis explores:

- Whether faster pit stops correlate with better finishing positions.
- Whether faster pit stops translate into gaining more places compared to the starting grid.
- How pit-stop performance varies among constructors across the years.

A series of statistical tests and visualizations—including Spearman’s rank-order correlation and ggpairs plot matrices—are used to uncover insights. A key feature is a year-wise comparison of median pit-stop durations by constructor via bar plots, highlighting trends in pit crew performance and field convergence.

## Project Contents

- **Quarto file:** Contains the full written blog post with embedded R code for data preparation, analysis, and visualization.
- **Data dictionary:** Detailed descriptions of all variables used from the Ergast dataset and their relevance to the analysis. This document aids understanding of the data structure and coding logic.
- **Data:** Raw CSV files downloaded from the Ergast database, including `pit_stops.csv`, `results.csv`, `races.csv`, `drivers.csv`, `constructors.csv`, and `status.csv`.

## Data Sources and Licensing

- Data is sourced from the [Ergast Developer API and database:](http://ergast.com/mrd/db/)
- The data covers Formula 1 race events, results, and pit stop timings from 2009 onwards.
- Use is permitted for educational and research purposes under Ergast’s non-commercial license terms.

## How to Run the Analysis

1. Place all relevant CSV data files in the `data/` folder.
2. Open the main Quarto document.
3. Run all code chunks to:
   - Load and merge data tables.
   - Filter data for the target seasons.
   - Calculate pit-stop durations in seconds and position gains.
   - Perform Spearman correlation tests.
   - Generate visualizations including correlation matrix plots and median pit-stop bar charts.
4. The final document includes written interpretation alongside the outputs.

## Notes

- Outliers and extremely long pit stops (>50 seconds) are filtered to avoid skewing results.
- The analysis focuses on four selected seasons to compare pit-stop impacts over time.
- The project uses consistent color palettes (`team_colors`) for constructors to maintain clarity in plots.

## Contact

For questions or further details, please reach out to:

**Jyovika Aswale**  
Master’s Student - Business Analytics - Monash 
Email: jasw0002@student.monash.edu