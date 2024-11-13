# Are We Alone? Project

## Overview
The **Are We Alone?** project explores patterns and trends in UFO sightings across the United States, examining factors such as geographic location, date, duration, and political regions. By clustering sightings and using demographic data, this project seeks to identify potential correlations with sociopolitical and environmental factors. The project uses interactive visualizations, machine learning models, and historical data analysis to deepen our understanding of UFO sighting patterns.

## Project Structure

- **Data Preprocessing and Cleaning**: The raw dataset undergoes several preprocessing steps to ensure data quality and consistency.
- **Data Exploration and Analysis**: Using clustering, seasonal patterns, and geographic data to analyze sightings over time.
- **Visualization**: Interactive maps and charts to visualize sighting trends by location, time, and shape.

## Notebooks

### `Final.ipynb`
- **Data Cleaning**: 
  - Converted columns to appropriate data types, especially `datetime` for dates and times.
  - Filtered sightings to include data from 1947 onward and only U.S. locations.
  - Removed ambiguous and irrelevant shapes and filtered out extreme outliers in sighting duration.

- **Analysis**: 
  - Explored trends in sightings over years, states, months, and seasons.
  - Identified "hotspot" states (e.g., California, Texas) with the highest sighting counts.
  - Observed peak sightings in summer months and during warmer seasons, potentially due to increased outdoor activity.
  - Used clustering algorithms to categorize sightings by geographic region, sighting duration, and reported UFO shape.

- **Visualization**:
  - Created bar charts to display the number of sightings by state, month, and shape.
  - Plotted sightings by season and created heatmaps for geographic distribution.
  - Generated an elbow curve to identify the optimal number of clusters for geographic analysis.

### `Untitled.ipynb`
- **Data Cleaning**: 
  - Converted `duration (seconds)` column to numeric, filtered durations to realistic ranges (1 to 7200 seconds), and removed any irrelevant columns.
  - Stored cleaned data in a local SQLite database for further processing and analysis.

- **Top City Analysis**:
  - Analyzed the top 10 cities by sighting counts, identifying which cities had the highest frequency of sightings over time.

## Key Findings
- **Temporal Trends**: Sightings peaked in summer months and during warmer seasons, possibly due to increased outdoor activity.
- **Geographic Hotspots**: States with large populations or outdoor activity, such as California and Texas, reported more sightings.
- **Sociopolitical Context**: Incorporated political affiliation of states to explore correlations between sighting frequency and state politics.
- **Common Shapes and Durations**: Specific shapes like "circle" and "triangle" were frequently reported, and sightings were generally short in duration, likely influenced by cultural perceptions of UFOs.

## Tools and Libraries
- **Python**: Primary language used for data analysis and visualization.
- **Pandas**: Data manipulation and cleaning.
- **Matplotlib, Seaborn, hvplot**: Visualization libraries for creating charts, maps, and plots.
- **Geoviews & Panel**: Tools for creating interactive geographic maps and dashboards.
- **Sklearn**: Machine learning library for clustering and scaling.
- **SQLite**: Local database for data storage and query management.

## Project Setup
To run this project locally:
1. Clone this repository and install the necessary dependencies.
2. Set up a virtual environment and install required packages from `requirements.txt`.
3. Run the notebooks sequentially for data preprocessing, analysis, and visualization.

## Future Improvements
- **Incorporate Real-Time Data**: Integrate new sighting data as it becomes available.
- **Advanced Modeling**: Explore other machine learning models for pattern recognition.
- **Enhanced Visualizations**: Add more interactive visualizations to explore patterns dynamically.
