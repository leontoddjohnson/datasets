# Beer Reviews Dataset

## Description

This is the [Beer Reviews](https://www.kaggle.com/datasets/rdoume/beerreviews) data set from Kaggle. It contains over 1.5 million reviews of various beers, including information about the beer style, brewery, and user ratings. According to the documentation, the data is originally from the BeerAdvocate website. Further, it was apparently used in the [*How to hire and test for data skills: A one-size-fits-all interview kit*](https://www.oreilly.com/videos/strata-data-conference/9781491976326/9781491976326-video316337/) talk at the [2017 Strata Data Conference in NYC](https://www.oreilly.com/videos/-/9781491976326/).

## Loading the data

The raw data is a zipped CSV file, so it is recommended to be loaded as follows in Python:

```python
url = "https://raw.githubusercontent.com/leontoddjohnson/datasets/main/data/beer_reviews/beer_reviews.csv.zip"
df_raw = pd.read_csv(url, compression='zip', low_memory=False)
```