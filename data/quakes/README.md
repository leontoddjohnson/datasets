# Quakes Dataset

> Current as of November 2023

## Description

This dataset was queried from the [USGS Earthquake Catalog](https://earthquake.usgs.gov/earthquakes/search/) with the following settings:

- **Magnitude**: Custom (5 or more)
- **Date & Time**:
  - Start: 2013-01-01
  - End: 2023-11-04
- **Geographic Region**: World
- **Output Options**: CSV

### Usage

(Using tidyverse packages.)

```R
url_ <- "https://raw.githubusercontent.com/leontoddjohnson/datasets/main/data/quakes/quakes.csv"
quakes <- read_delim(url_, delim = ",")
```

### Details

See the documentation (linked above) for more information on the format and columns.

## TODO

- [ ] N/A