# COVID Death Dataset

## Description

This dataset is a **subset** of the *Provisional COVID-19 Deaths by County, and Race and Hispanic Origin* data set. For more information on this data, see the [documentation here](https://data.cdc.gov/NCHS/Provisional-COVID-19-Deaths-by-County-and-Race-and/k8wy-p9cg/about_data).

## Data Cleaning

The raw data was imported from the above source, and cleaned using the following procedure:

```python
df = pd.read_csv(".../covid_2023.csv", dtype={"FIPS Code": str})

df.rename(columns=lambda s: s.lower().replace('-', '').replace(' ', '_'), inplace=True)

df = df[['state', 'county_name', 'fips_code', 'total_deaths', 'covid19_deaths']].drop_duplicates()
```

### Usage

```R
url_ <- "https://raw.githubusercontent.com/leontoddjohnson/datasets/main/data/covid_2023/covid_2023.csv"
marketing <- read_delim(url_, delim = ",")
```