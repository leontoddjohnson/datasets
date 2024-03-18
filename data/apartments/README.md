# Apartments Dataset

> This dataset is strictly for educational use!

## Description

This apartments dataset contains rows of theoretical apartments listed in New York City (NYC) and San Francisco (SF). It was built for the purposes of education.

### Usage

```R
url_ <- "https://raw.githubusercontent.com/leontoddjohnson/datasets/main/data/apartments/apartments.csv"
marketing <- read_delim(url_, delim = ",")
```

### Format

The `apartments` dataset contains `492` rows (each row is a different apartment) and `8` columns:

- `in_sf`: a boolean value which is 1 when the apartment is located in SF
- `beds`: number of bedrooms in the apartment
- `bath`: number of bathrooms
- `price`: listing price for the apartment
  
- `year_built`: the year the property was built
  - Suppose this is the year that the apartment was designated as its own space. If one apartment was originally part of another apartment (say the property got split up), then those two apartments would have two different values in this column.

- `sqft`: The square footage for the apartment
- `price_per_sqft`: This is just `round(price / sqft)`
- `elevation`: the elevation of the apartment in feet above sea level.



### Details

Original origin unknown ...

## TODO

- [ ] N/A