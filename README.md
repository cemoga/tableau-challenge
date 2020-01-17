# Citibike Metrics

## Project description

The purpose of this project is to aggregate, describe and analize phenomena found in the Citibike program in New York City.

## Link to the visualizations

- [Tableau Public](https://public.tableau.com/profile/cesar.mosquera#!/vizhome/Citibike_15789352935200/CitibikeProgramMetrics-Story).

### Steps

1. Use of `Python` to aggregate data from the [Citibike Data Page](https://s3.amazonaws.com/tripdata/index.html). Files from 2017 until the end of 2019 were used

    - The `CSV` files in the `data_original` folder were uploaded to `Pandas Pandas DataFrames`
    - The headers of the `Pandas DataFrames` were changed to be the same for all the `CSV` files
    - The `Pandas DataFrames` with the standardized headers were exported to the `data_modified` folder
    - The `CSV` files in the modified folder were uploaded to a single `Pandas DataFrame`

2. Elimination of outliers. By using `Python`, bike rides taking longer than 3 hours were eliminated as outliers. After pre-analysis, these trips were made to maintenance stations, were out of the scope of the analysis and distorted the conclusions

    - The `Pandas DataFrame` containing the data of all the months was filtered to eliminate the outliers
    - New aggregated `Pandas DataFrames` were created summarizing the data by `costumer tye and gender`, by `starting station name` and for `stoping station name
    - Small `CSV` files, the product of the aggregation, were exported to the `data_output` folder

3. Use of `Tableau` to describe and analyze the phenomena from the data by creating `visualizations`, `dashboards`, and a `story`

### Screenshots

### Analysis

The most popular Citibike stations are next to huge transportation hubs (Grand Central Terminal and Penn Station) and have bike lanes nearby. This situation is summarized in the chart below for the most popular Citibike Stations for the timespan of the analysis.

![Popular Station Analysis](screenshots/popular_station_analysis.png "Popular Station Analysis")