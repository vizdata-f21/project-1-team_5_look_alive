Is soybean use driving global deforestation?
================
by Team 5 Look Alive

## Introduction

Our data comes originally from the UN Food and Agriculture
Organization’s Forest Resources Assessment. “Since year-to-year
changes in forest cover can be volatile, the UN FAO provide this annual
data averaged over five-year periods.” It measures the area of forests
over time in countries around the world. It also holds more detailed
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

## What countries are seeing the most deforestation within their borders, and what is causing this deforestation?

### Introduction

These ideas stuck us as the most essential elements of deforestation,
and gaining an understanding of the complexities of deforestation
depends on becoming familiar with these concepts.

### Approach

In this question, we planned on exploring three things: the who, the
what, and the why of deforestation. First, we chose to use a line plot
to examine trends over time in deforestation. This would allow us to get
a rough understanding of how many countries are facing the most
deforestation and examine the most deforested country’s data, using a
cumulative line plot of deforestation and a bar plot to compare across
years. From here, we could then examine the “what”. To do this, we
decided to compare the proportions with an area plot. This gave us the
opportunity to showcase which causes are the most impactful in Brazil’s
deforestation. Finally, to understand the “why” of deforestation, we
selected to examine one of the leading causes of deforestation in
Brazil. Using line plots again allowed us to highlight which regions and
countries are most influential in driving soybean production globally.

Putting all of these factors together gives us a basic understanding of
global deforestation.

### Analysis

#### Figure 1

<img src="README_files/figure-gfm/cumulative_brazil_only-1.png" title="Brazil lost 30m hectares of forest from 2000 to 2013." alt="Brazil lost 30m hectares of forest from 2000 to 2013."  />

#### Figure 2

<img src="README_files/figure-gfm/drivers_of_brazil_deforstation-1.png" title="Pasture is the most common cause of deforestation in Brazil, " alt="Pasture is the most common cause of deforestation in Brazil, " width="70%" />

#### Figure 3

<img src="README_files/figure-gfm/soybean_use_countries-1.png" title="China, US, Brazil, Argentina identified as countries that use the most soybean." alt="China, US, Brazil, Argentina identified as countries that use the most soybean." width="70%" />

### Discussion

Figure 1 portrays the amount of lost forest in Brazil in the span of 13
years, from 2000 to 2013. The loss is striking at over 30 million
hectares (300,000 square km, for reference). The figure does show a
concave trend, which shows that the loss of forest is not exponential,
signaling that there may be hope in a continued flattening of this line
of forest loss. It is interesting to consider what factors may have
contributed to these trends within Brazil. Lawmaking and leadership will
play a role in a country’s development, meaning that it would be
fascinating to gather this same data from Jair Bolsonaro’s current reign
as Brazil’s president and compare it to the trends under Brazilian
presidents who led during the time period of this plot, such as Lula de
Silva, who served as president from 2003-2010 in Brazil (Wikipedia,
Brazilian Presidents).

Figure 2 offers a view of the causes of Brazilian loss of forest. The
most common reason for removal of forest in Brazil is to clear space for
land to be used as pasture. Other big causes of loss of forest include
fire, logging, small-scale farming, and commercial crops. Fires
fluctuate wildly on the plot, demonstrating their lack of predictability
and their destructive nature. Global warming and human activity may be
factors that contributes to the increased danger of forest fires in the
Amazon (Bush et. al. 2008). One important commercial crop is soybean,
which we chose to analyze further, guided by our retrieval of data on
soybean use.

Figure 3 gives a look into which countries are the largest consumers of
soybean, which in turn increases demand for soybean and drives
deforestation. China, the United States, Brazil, and Argentina were
found to be the most prevalent soybean consumers. Argentina was the most
surprising to us, but we found that soybean is a vital crop to
Argentina, which incentivizes the use of soybean after its growth
(croplife, Soybeans in Argentina).

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

Ritchie, H. and Roser, M. 2021, “Forests and Deforestation”. Published
online at OurWorldInData.org. Retrieved from:
‘<https://ourworldindata.org/forests-and-deforestation>’ on September
13, 2021 \[Online Resource\]

## References

1.  [Brazilian
    Presidents](https://en.wikipedia.org/wiki/List_of_presidents_of_Brazil)
2.  Bush, M. B., Silman, M. R., McMichael, C., & Saatchi, S. (2008).
    Fire, climate change and biodiversity in Amazonia: a Late-Holocene
    perspective. Philosophical transactions of the Royal Society of
    London. Series B, Biological sciences, 363(1498), 1795–1802.
    <https://doi.org/10.1098/rstb.2007.0014>
3.  [Soybeans in
    Argentina](https://croplife.org/news-views/sharing-the-story/soybeans-from-argentina/#:~:text=The%20country%20grew%2020%20million,cereal%2C%20automotive%20and%20petrochemical%20exports.&text=The%20health%20of%20the%20soybean,therefore%2C%20of%20great%20national%20interest.)
4.  [Our World in
    Data](https://ourworldindata.org/forests-and-deforestation)
5.  [Deforestation](https://ourworldindata.org/deforestation)  
6.  [Share of forest area](https://ourworldindata.org/forest-area)  
7.  [Drivers of
    deforestation](https://ourworldindata.org/drivers-of-deforestation)  
8.  [Deforestation by
    commodity](https://ourworldindata.org/grapher/deforestation-by-commodity)  
9.  [Soybean production and use](https://ourworldindata.org/soy)  
10. [Palm oil production](https://ourworldindata.org/palm-oil)
