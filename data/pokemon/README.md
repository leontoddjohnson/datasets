# Pokémon Dataset

> This dataset is strictly for educational use!

## Description

This dataset is simulated for the following hypothetical situation.

**Background:**You've just been hired as a Pokémon researcher, and your assignment is to maintain a dataset of sightings from trainers worldwide. You expect future inputs may be duplicate entries, and there may be missing values or inconsistent formats. These sorts of entries can cause the system to crash, so you need to build a validation process for newly recieved data.

**Objective:** Implement a system that validates new Pokémon entries, handling errors and ensuring all necessary information is present.

### Usage

```R
url_ <- "https://raw.githubusercontent.com/leontoddjohnson/datasets/main/data/pokemon/pokemon_entries.csv"
pokemon <- read_delim(url_, delim = ",")
```

```python
url_ = "https://raw.githubusercontent.com/leontoddjohnson/datasets/main/data/pokemon/pokemon_entries.csv"
pokemon <- pd.read_csv(url_)
```

### Notes

These data include a collection of **first** sightings from various trainers.

**Input Requirements**

- Deny duplicates. If the `pokemon_id`-`trainer_name`-`seen_time` combination already exists, then this is a duplicate.
- The `pokemon_type` must be one of the following: 'Water', 'Fire', 'Grass', 'Earth', 'Normal', or it can be unknown.
    - These must be capitalized.
- The `pokemon_id` cannot be negative, and it must be an integer.
- Recall that the current entry data includes **first** sightings from trainers. So, a new sighting for a trainer cannot be before a date already in the dataset.
    - For example: Trainer_35 cannot have seen a new pokemon before 2023-12-05 at noon.

## TODO

- [ ] Design better trainer names.