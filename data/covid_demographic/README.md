# COVID by Demographic

## Description

This is the **raw** dataset, pulled directly from [the associated CDC webpage](https://data.cdc.gov/Public-Health-Surveillance/COVID-19-Weekly-Cases-and-Deaths-by-Age-Race-Ethni/hrdz-jaxc/about_data). Note: **each row is a week for a jurisdiction** (see below).

## Caveats to the Documentation

A few things to note about this data that are not immediately clear in the documentation:

- It is assumed that by "jurisdiction", we mean one of the ten US regions listed [here](https://en.wikipedia.org/wiki/List_of_regions_of_the_United_States#Regions_and_office_locations).
- For the numeric columns, pay close attention to what a missing value means ...
- Each of the categorical columns have an "Overall" value that *presumably* contains "duplicates" of the other rows for that juristiction-week.
    - That said, the documentation does say *"Records with unknown or missing sex, age, or race and ethnicity and of multiple, non-Hispanic race and ethnicity are included in case and death totals."*, so there are likely rows in the "Overall" totals that are *not* duplicated elsewhere.
    - In general, it might be a good idea to either choose the "Overall" data, or everything else.

### Usage (in R)

```R
url_ <- "https://raw.githubusercontent.com/leontoddjohnson/datasets/main/data/covid_demographic/covid_demographic.csv"
covid <- read_delim(url_, delim = ",")
```

## TODO

- [ ] Consider uploading a separarte "clean version"
- [ ] Investigate the claim about duplicated data in "Overall" categories
