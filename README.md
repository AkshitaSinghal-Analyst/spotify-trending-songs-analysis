# Spotify Trending Songs Analysis

## Project Overview
This project analyzes Spotify trending songs using streaming statistics, chart rankings, artist information, and genre data to identify music trends, popularity patterns, and chart performance.
The analysis covers exploratory data analysis, feature engineering, correlation analysis, song classification, and linear regression.

## Objective
The main objectives of this project are:
- Analyze Spotify trending songs based on streams and rankings
- Identify top-performing songs, artists, and genres
- Study relationships between rankings, streams, and chart performance
- Classify songs based on their chart longevity
- Apply regression analysis to predict streaming performance

## Dataset
The dataset contains 2,200 Spotify chart entries spanning 11 weeks and 11 columns.
The dataset includes information such as:
- Week and chart rank
- Artist names and track names
- Music source
- Peak rank and previous rank
- Weeks on chart
- Streams
- Genre
No missing values were found in the dataset. :contentReference[oaicite:1]{index=1}

## Tools Used
- Python
- Microsoft Excel

## Analysis Performed
- Data understanding and descriptive statistics
- Top 10 most streamed songs analysis
- Top artists by total streams
- Genre-wise streaming analysis
- Streams vs Weeks on Chart analysis
- Rank vs Streams analysis
- Correlation analysis
- Song classification
- Top stable songs analysis
- Linear regression modelling
- Actual vs Predicted Streams analysis

## Feature Engineering
Three derived features were created during the analysis:
- **Popularity Score** = Streams ÷ Rank
- **Stability Score** = Weeks on Chart × Streams
- **Rank Improvement** = Previous Rank − Current Rank
These features were used to analyze streaming popularity, chart stability, and ranking momentum. :contentReference[oaicite:2]{index=2}

## Song Classification
Songs were classified into three categories based on their weeks on chart:
- **Evergreen Hit** — 30+ weeks on chart
- **Trending Song** — 15 to 29 weeks
- **New Viral Song** — under 15 weeks
The classification was used to understand differences in chart longevity and audience engagement. :contentReference[oaicite:3]{index=3}

## Regression Model
A Linear Regression model was trained to predict streams using:
- Rank
- Peak Rank
- Weeks on Chart
- Popularity Score
The dataset was divided into 80% training data and 20% test data.

### Model Performance
- **R² Score:** 0.857
- **MAE:** 308,031
- **MSE:** 164,955,639,128
The model explained approximately 85.7% of the variance in streams using the selected chart-based features. :contentReference[oaicite:4]{index=4}

## Key Findings
- Higher-ranked songs generally received more streams.
- Rank and streams showed a strong negative correlation of **-0.786**.
- Longer chart presence generally corresponded with higher streaming performance.
- Weeks on Chart and Stability Score showed a strong positive correlation of **0.891**.
- Streams and Popularity Score showed a positive correlation of **0.696**.
- Bollywood Romantic, Indie Pop, and Punjabi Hip-Hop/Rap were among the leading genres by total streams.
- The dataset contained a mix of viral tracks, trending songs, and longer-running evergreen hits. :contentReference[oaicite:5]{index=5} :contentReference[oaicite:6]{index=6}

## Repository Contents
- `data/` — Spotify dataset used for analysis
- `analysis/` — Analysis PDF
- `report/` — Detailed findings report
