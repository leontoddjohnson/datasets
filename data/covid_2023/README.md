# COVID Death Dataset

## Description

This dataset is the *Provisional COVID-19 Deaths by County, and Race and Hispanic Origin* data set. For more information on this data, see the [documentation here](https://data.cdc.gov/NCHS/Provisional-COVID-19-Deaths-by-County-and-Race-and/k8wy-p9cg/about_data).

### Usage

```R
url_ <- "https://raw.githubusercontent.com/leontoddjohnson/datasets/main/data/covid_2023/covid_2023.csv"
marketing <- read_delim(url_, delim = ",")
```