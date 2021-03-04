# Lincoln-Douglas Debate Dataset

Compiled list of varsity Lincoln-Douglas (LD) debate results at bid distributing tournaments.

## Data

This dataset includes six seasons, 18 topics, 252 tournaments, and 76,296 debates.

The following information was recorded for each debate:

* Season
 * 2015 - 2016
 * 2016 - 2017
 * 2017 - 2018
 * 2018 - 2019
 * 2019 - 2020
 * 2020 - 2021
* Topic
 * SO - September October
 * ND - November December
 * JF - January February
* Bid Level
 * F - Finals
 * S - Semifinals
 * Q - Quarterfinals
 * O - Octo-finals
 * TOC - Tournament of Champions
* Tournament
 * Name of tournament as displayed on the tournament bid list
* Round
 * Name of the round the debate occured in
* Aff
 * Debater UUID 
* Neg
 * Debater UUID
* Winner
 * aff
 * neg

### Sources

List of bid distributing tournaments was obtained from the [University of Kentucky's Tournament of Champions website](https://ci.uky.edu/UKDebate/ld-bid-tournaments-0).

Detailed information on LD rounds was obtained from [tabroom.com](tabroom.com) by scraping tournament round result pages.

## Usage

Using `python` and the `pandas` package is the recommended method to access the dataset.

Install the requirements with: `pip install pandas`.

```
import pandas as pd

# load data
data = pd.read_csv('data.csv')

# select current season
data = data.loc[data['Season'] == '2020 - 2021']
```

## Citing
This dataset is made available under the [Open Data Commons Attribution License](https://opendatacommons.org/licenses/by/1-0/). Crediting Sachin Shah and tabroom.com is expected.

Shah, Sachin (2021). Lincoln-Douglas Debate Dataset [Data file]. Retrieved from https://github.com/inventshah/LD-data