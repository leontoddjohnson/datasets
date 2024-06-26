# datasets

This repository serves to offer a collection of small datasets, for educational purposes. Each dataset has a purpose and documentation.

To access most of these datasets, you can use the following URL:

```
https://raw.githubusercontent.com/leontoddjohnson/datasets/main/<pathtofile>
```

## list of datasets without a README file

- [ames](./data/ames.csv) ([documentation](https://jse.amstat.org/v19n3/decock/DataDocumentation.txt))
- [coffee](./data/coffee_analysis.csv) ([documentation](https://www.kaggle.com/datasets/schmoyote/coffee-reviews-dataset/))
- [titanic](./data/titanic.csv) ([documentation](https://www.kaggle.com/competitions/titanic/data))
- [uk_retail](./data/uk_retail.csv) ([documentation](https://archive.ics.uci.edu/dataset/352/online+retail))

# data repositories

Alternatively, below is a list of data repositories that tend to be pretty clean and manageable, and most have decent documentation:

- [ggplot2 datasets](https://ggplot2.tidyverse.org/reference/#data) (installed during **R Setup**)
- [tidytuesday repository](https://github.com/rfordatascience/tidytuesday/tree/master) (using R to import data)
  - An easy way to find datasets in this repository is to use the *"Type [/] to search"* search bar at the top of the main repository page, and select *"Search in this repository".*
  - Then, select *"CSV"* from the filtration side-bar on the left.
- [CDC Data Catalog](https://data.cdc.gov/browse)
- [UCI Regression Datasets](https://archive.ics.uci.edu/datasets). To use these, you'll need to:
  1. Get the column names from the documentation on the main dataset page (or the *.names* file), and create a vector of those names *in order*.
  2. Use `read_delim` in R, setting the `file` to be the path to the *.data* file, and specifying `col_names` to be the column names vector from above. You may also need to adjust `delim` depending on what you see in the *.data* file (it could be a space, comma, semicolon, tab, etc.)
- [pudding.cool data](https://github.com/the-pudding/data) (used for articles on [pudding.cool](https://pudding.cool/))
  - If you use a Pudding dataset, try to illustrate something which is not already included in its corresponding pudding article
- [FiveThirtyEight data repository](https://github.com/fivethirtyeight/data) (used for articles on their [website](https://fivethirtyeight.com/))
- [World Health Organization Data Collections](https://www.who.int/data/collections)
  - Sometimes, getting to the data might take a bit of digging ...
- [The World Bank Databases](https://databank.worldbank.org/databases) (use the below instructions to access the data)
  1. Select a database.
  2. Select the "Variables" tab (on the upper left), and choose the data you're interested in.
  3. Select the "Layout" tab, and click "Orientation". For "Series", select "Column" from the dropdown box. For *all* other factors, select "Row" from the dropdown box.
  4. Click "Apply Changes" in the pop-up box.
  5. Click the "Download options" in the upper right corner, and select "CSV". Boom.

*Note: [Kaggle](https://www.kaggle.com/datasets/) and [data.world](https://data.world/datasets/open-data) also have myriad datasets, but they can get messy, and their documentation is often questionable at best. Just be mindful if you choose to use either of these sources.*
