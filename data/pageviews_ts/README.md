# Page Views (Time Series)

> Current as of April 2024

## Description

This dataset was queried from the [Wikipedia Pageviews API](https://pageviews.wmcloud.org/?project=en.wikipedia.org&platform=all-access&agent=user&redirects=0&start=2019-01-01&end=2024-04-01&pages=Time_series) (with the given settings).

It is a daily time series of webpage views of the "Time Series" Wikipedia page over an approximately 5 year period.

### Usage

(Using tidyverse packages.)

```R
url_ <- "https://raw.githubusercontent.com/leontoddjohnson/datasets/main/data/pageviews_ts/pageviews_ts.csv"
pageviews_ts <- read_delim(url_, delim = ",")
```

### Details

See the [Pageviews documentation](https://meta.wikimedia.org/wiki/Pageviews_Analysis) for more information on the data.

## TODO

- [ ] N/A