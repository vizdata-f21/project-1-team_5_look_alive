Project Proposal
================
Team 5 Look Alive

## Dataset

``` r
forest <- read.csv("../data/forest.csv")
forest_area <- read.csv("../data/forest_area.csv")
brazil_loss <- read.csv("../data/brazil_loss.csv")
vegetable_oil <- read.csv("../data/vegetable_oil.csv")
soybean_use <- read.csv("../data/soybean_use.csv")
```

We chose the global deforestation data from
<https://github.com/rfordatascience/tidytuesday/blob/master/data/2021/2021-04-06/readme.md>,
which was sourced from Our World in Data.

The dataset has 5 elements: `forest`, `forest_area`, `brazil_loss`,
`soybean_use`, and `vegetable_oil`. The set `forest` contains the change
every 5 years in for forest area in conversion. It comes originally from
the UN Food and Agriculture Organization’s Forest Resources Assessment.
“Since year-to-year changes in forest cover can be volatile, the UN
FAO provide this annual data averaged over five-year periods.”
`forest_area` contains the change in global forest area as a percent of
global forest area. `brazil_loss` contains the loss of Brazilian forest
due to specific types of deforestation, such as `fire` and
`small_scale_clearing`. `soybean_use` contains the soybean production
and use by year and by country. Finally, the set `vegetable_oil`
contains vegetable oil production by crop type and year.

We chose this dataset because we were interested to see the relationship
between soybean production on deforestation in Brazil and global
deforestation. The data also had few missing values, and multiple
datasets, so we were able to brainstorm several ideas we’d be interested
in.

## Questions

Question one: What is the relationship between global soybean use and
deforestation in Brazil? What countries are driving the growing of
Brazil’s commercial soybean crops?

Question two: How does the proportions of soybean production used for
human food versus for feeding animal change over time? Is this change in
proportions related to global deforestation development over time?

## Analysis plan

### Plan for Question One:

We want to plot global soybean use over time as compared to Brazil’s
deforestation (Brazil is the world’s leader in soybean export). The
datasets we will combine for this plot are `brazil_loss`, `soybean_use`
and `forest_area`.

Plan for soybean use over time: create new variable `total_use` that
combines `human_food`, `animal_feed`, and `processed` for each
observation. Group by `year` to create a dataset with the total global
use per year. Plot this as a line chart.

Plan for Brazil’s deforestation: Filter Brazil observations from
`forest_area` dataset. Plot as a line chart.

Based on what we see above, we may want to look at some more specific
variables to see if they develop into a more interesting story. The
other things we will consider looking at are looking at Brazil’s
deforestation *specifically due to commercial crops* (which would be
`commercial crops` from the `brazil_loss` dataset), and showing which
countries are using the most soybean. We also want to look at the
differentiation between types of use, how they have developed over time
and compared to deforestation, which led us to our second question.

### Plan for Question Two:

We want to examine the proportions of soybean production used for human
food versus for feeding animal change over time and whether this change
in proportions is related to global deforestation development over time.
The datasets we will use for this question are `soybean_use` and
`forest_area`.

Start by grouping all entries in `soybean_use` by decades. For each
decade category, add up the values for all entries under `human_food`,
`animal_feed`, and `processed`.

Create new variables `human_prop` and `animal_prop` that represent the
proportions of soybean production used for human food and for animal
feed out of the total each decade.

Plot `human_prop` and `animal_prop` as dots in a graph where the x-axis
represents `decade` and the y-axis represents proportion percentage
between 0 to 1. Connect all dots under each variable - `human_prop` and
`animal_prop` - with lines in differentiating shape and color.

Plot percent of global forest area, `forest_area`, as points in the
above graph and connect the dots with a different colored line. Observe
and compare the lines.
