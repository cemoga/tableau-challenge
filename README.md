# Citibike Metrics

## Project description

Aggregating, describing and analizing phenomea found in the Citibike program in New York City.

### Steps

1. Using `Python` to aggregate data from the [Citibike Data Page](https://s3.amazonaws.com/tripdata/index.html). Files from 2017 until the end of 2019 were used.

    - The `CSV`files in the `data_original` folder were uploaded to `Pandas` `dataframes`.
    - The headers of the `dataframes`were changed to be the same for all the `csv` files.
    - The `dataframes` with the standardized headers were exported to the `data_modified` folder.
    - The `CSV`files in the modified folder were uploaded to a single `dataframe`.

2. Eliminating outliers. By using `Python`, bike rides taking longer than 3 hours were eliminated as outliers. After pre-analysis, these trips were made to maintainance stations, were out of the scope of the analysis and distorted the conclusions.

    - The `dataframe` containing the data of all the months was filtered to eliminate the outliers.
    - New `aggregated dataframes` were created summarizing the data by `costumer tye and gender`, by `starting station name` and for `stoping station name.
    - Small product of the aggregation `CSV`files were exported to the `data_output` folder.

3. Using `Tableau`to describe and analyze the phenomena from the data by creating `visualizations`, `dashboards`and a `story`.

### Screenshots
