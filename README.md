# Tweeter-Data-Analysis
This notebook is focused on analyzing Twitter data. It loads raw JSON/CSV datasets, cleans them, and performs exploratory data analysis (EDA) with visualizations. It also applies statistical tests and geographic mapping to extract insights about tweet distributions, user behavior, and trends.\
🔑 Step-by-Step Breakdown

Import Libraries

Uses numpy, pandas, matplotlib, scipy, geopandas, and shapely for data wrangling, plotting, and geospatial analysis.

Load Data

Reads JSON/CSV Twitter datasets (e.g., merged_created_at.csv, merged_id_str.csv, and raw geoEurope files).

Data includes created_at, id, in_reply_to_user_id_str, and other tweet metadata.

Data Cleaning

Handles missing values (df.isnull().sum()).

Converts created_at into datetime format.

Merges multiple datasets (pd.concat) to create a comprehensive DataFrame.

Exploratory Data Analysis (EDA)

Counts tweets per day and user.

Identifies top users with the highest tweet activity.

Plots histograms showing tweets per user.

Visualization

Line plots of tweet frequency over time.

Word clouds to visualize most common words.

Geographic visualization: mapping tweets to European regions using GeoJSON.

Heatmaps for regional activity.

Statistical Analysis

Applies Mann-Whitney U test to compare weekday vs. weekend tweet distributions.

Tests statistical significance of tweet patterns.

Final Outputs

Histograms, time series plots, and geospatial maps.

Insights into user behavior and tweet trends across Europe.
