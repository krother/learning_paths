
# Time Series

## Lesson Goal:

Students interpret time series data

## Time Frame:

135'

## Key Concepts:

* random walk
* trend
* seasonality
* noise
* diff
* pct_change or log
* lag
* autocorrelation
* rolling mean

## Warmup:

* look at good/bad  line plots and discuss what makes them good or bad
* show the plot of a time series. Ask students what patterns they see.

## Content Delivery:

* brainstorm examples of time series
* give usage examples why organizations are interested in time series data
* plot a time series
* make sure the x-axis contains proper timestamps
* decompose: remove the trend with a diff
* decompose: remove growth with percentage change
* decompose: identify seasonality with an autocorrelation plot
* plot the residual pattern or noise after removing everything else

## Material:

for plotting and decomposition use either of:

- the seaborn flights dataset (clear seasonality)
- bitcoin data (information changes a lot on the log scale)
- [time series in pandas](https://krother.github.io/pandas_go_to_space/time_series/README.html)
- [climate stripes exercise](https://krother.github.io/pandas_go_to_space/challenges/climate_stripes/README.html)


## Comments:

TODO: it should be possible to come up with an easy game that generates time seeries data. The time series of a dice roll is rather shallow. 