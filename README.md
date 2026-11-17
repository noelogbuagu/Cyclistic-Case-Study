# Cyclistic Case Study

A case study in R, done after the Google Data Analytics professional certificate. It analyses twelve months of bike-share trip data (September 2020 to August 2021) for the fictional company Cyclistic, comparing how annual members and casual riders use the service.

## Layout

| File | Purpose |
|---|---|
| `cyclistic-case_study.Rmd` | The write-up: R Markdown with narrative, code and charts |
| `cyclistic-case_study.html` | The rendered report. Open this to read the result without running anything |
| `cyclistic_data_exploration.R` | The same data work as a plain R script |

## What the analysis does

1. **Prepare the environment** by loading the packages (`tidyverse`, `lubridate`, `janitor`, `skimr`, `here`, `geodist`, `ggmap`).
2. **Load and combine** the 12 monthly trip files.
3. **Clean:** rename columns (`member_casual` to `rider_type`, `rideable_type` to `bike_type`), parse dates and times, and derive ride length, hour, weekday, month, season and distance covered.
4. **Analyse and visualize** rider type by number of rides, time of day, ride duration and ride location (station maps).

## Running it

The monthly trip CSVs are not in the repo. The code expects them in a `data_sources/` folder, named like `202009-divvy-tripdata.csv`. They are the public Divvy trip data. The map section also needs a Google Maps API key registered with `ggmap`.

Install the packages listed above, then knit `cyclistic-case_study.Rmd` in RStudio.
