Deforestation Over Time
================
by Team 5 Look Alive

## Introduction

Our data comes originally from the UN Food and Agriculture
Organization’s Forest Resources Assessment. “Since year-to-year changes
in forest cover can be volatile, the UN FAO provide this annual data
averaged over five-year periods.” It measures the area of forests over
time in countries around the world. It also holds more detailed
information about the loss of Brazilian forest over time. The data
further holds data about soybean production and vegetable oil production
by year and country.

The dataset has 5 elements: `forest`, `forest_area`, `brazil_loss`,
`soybean_use`, and `vegetable_oil`. The set `forest` contains the change
every 5 years in for forest area in conversion. `forest_area` contains
the change in global forest area as a percent of global forest area.
`brazil_loss` contains the loss of Brazilian forest due to specific
types of deforestation, such as `fire` and `small_scale_clearing`.
`soybean_use` contains the soybean production and use by year and by
country. Finally, the set `vegetable_oil` contains vegetable oil
production by crop type and year.

## What is the relationship between global soybean use and deforestation in Brazil? What countries are driving the growing of Brazil’s commercial soybean crops?

### Introduction

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

### Approach

Based on what we see above, we may want to look at some more specific
variables to see if they develop into a more interesting story. The
other things we will consider looking at are looking at Brazil’s
deforestation *specifically due to commercial crops* (which would be
`commercial crops` from the `brazil_loss` dataset), and showing which
countries are using the most soybean. We also want to look at the
differentiation between types of use, how they have developed over time
and compared to deforestation, which led us to our second question.

### Analysis

(2-3 code blocks, 2 figures, text/code comments as needed) In this
section, provide the code that generates your plots. Use scale functions
to provide nice axis labels and guides. You are welcome to use theme
functions to customize the appearance of your plot, but you are not
required to do so. All plots must be made with ggplot2. Do not use base
R or lattice plotting functions.

### Discussion

(1-3 paragraphs) In the Discussion section, interpret the results of
your analysis. Identify any trends revealed (or not revealed) by the
plots. Speculate about why the data looks the way it does.

## How does the proportions of soybean production used for human food versus for feeding animal change over time? Is this change in proportions related to global deforestation?

### Introduction

We want to examine the proportions of soybean production used for human
food versus for feeding animal change over time and whether this change
in proportions is related to global deforestation development over time.
The datasets we will use for this question are `soybean_use` and
`forest_area`.

### Approach

(1-2 paragraphs) Describe what types of plots you are going to make to
address your question. For each plot, provide a clear explanation as to
why this plot (e.g. boxplot, barplot, histogram, etc.) is best for
providing the information you are asking about. The two plots should be
of different types, and at least one of the two plots needs to use
either color mapping or facets.

### Analysis

(2-3 code blocks, 2 figures, text/code comments as needed) In this
section, provide the code that generates your plots. Use scale functions
to provide nice axis labels and guides. You are welcome to use theme
functions to customize the appearance of your plot, but you are not
required to do so. All plots must be made with ggplot2. Do not use base
R or lattice plotting functions.

### Discussion

(1-3 paragraphs) In the Discussion section, interpret the results of
your analysis. Identify any trends revealed (or not revealed) by the
plots. Speculate about why the data looks the way it does.

## Presentation

Our presentation can be found [here](presentation/presentation.html).

## Data

Include a citation for your data here. See
<http://libraryguides.vu.edu.au/c.php?g=386501&p=4347840> for guidance
on proper citation for datasets. If you got your data off the web, make
sure to note the retrieval date.

## References

List any references here. You should, at a minimum, list your data
source.
