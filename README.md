# Ireland Weather Data Analysis Project

## Project Overview
This project performs an exploratory analysis of Irish weather data spanning nearly 60 years. It focuses on four climate-related datasets:
- `wind.csv`: wind speed data
- `sunshine.csv`: sunshine duration data
- `temperature.csv`: temperature data
- `meteorological.csv`: general meteorological observations (including precipitation)

The analysis includes data preprocessing, missing value handling, dataset merging, trend exploration, and visualization of key relationships among weather variables.

## Key Files
- `R_final_tangjinchi.qmd`: main Quarto analysis document with data import, cleaning, merging, and visualization
- `R_final_tangjinchi.pdf`: exported PDF report from the Quarto document
- `Untitled.R`: supplementary R script
- `Rfinal.Rproj`: RStudio project file
- Data files: `wind.csv`, `sunshine.csv`, `temperature.csv`, `Meteorological.csv`

## Workflow
1. Read and convert the four raw datasets into `tibble` format
2. Compare dataset dimensions and identify differences in statistical labels
3. Split temperature and wind datasets by statistic label and rename the `VALUE` column
4. Merge datasets using `Meteorological.Weather.Station` and `Month` as keys
5. Convert month labels into standard date format and extract the year
6. Identify and remove stations with excessive missing values (e.g. Markree, Phoenix Park, Roches Point)
7. Analyze the final dataset `weather_main` for climate patterns and relationships

## Key Findings
- Ireland exhibits a temperate maritime climate with mild summers and cool winters
- Mean temperatures for January and July show a gradual rise of around 0.5–1°C over the past 60 years
- Wind speed and precipitation are positively correlated, while sunshine hours tend to decrease as wind speed and precipitation increase

## Tools and Dependencies
This project is implemented in R and is best viewed in RStudio. Main packages used include:
- `dplyr`
- `tibble`
- `lubridate`
- `purrr`
- `ggplot2`
- `knitr`

## How to Use
1. Open `R_final_tangjinchi.qmd` in RStudio.
2. Render the Quarto document to generate the report in PDF or HTML format.
3. Run individual code chunks inside RStudio to reproduce the analysis.

## Notes
The current repository focuses on the meteorological data analysis pipeline and visualization. Some earlier course work sections were removed to keep the project concise and relevant for a job application.