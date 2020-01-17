# Citibike Metrics

## Project description

Aggregating, describing and analyzing phenomena found in the Citibike program in New York City.

### Steps

1. Using `Python` to aggregate data from the [Citibike Data Page](https://s3.amazonaws.com/tripdata/index.html). Files from 2017 until the end of 2019 were used.

    - The `CSV` files in the `data_original` folder were uploaded to `Pandas Pandas DataFrames`.
    - The headers of the `Pandas DataFrames` were changed to be the same for all the `CSV` files.
    - The `Pandas DataFrames` with the standardized headers were exported to the `data_modified` folder.
    - The `CSV` files in the modified folder were uploaded to a single `Pandas DataFrame`.

2. Eliminating outliers. By using `Python`, bike rides taking longer than 3 hours were eliminated as outliers. After pre-analysis, these trips were made to maintenance stations, were out of the scope of the analysis and distorted the conclusions.

    - The `Pandas DataFrame` containing the data of all the months was filtered to eliminate the outliers.
    - New aggregated `Pandas DataFrames` were created summarizing the data by `costumer tye and gender`, by `starting station name` and for `stoping station name.
    - Small `CSV` files, the product of the aggregation, were exported to the `data_output` folder.

3. Using `Tableau` to describe and analyze the phenomena from the data by creating `visualizations`, `dashboards` and a `story`.

### Screenshots
