---
title: "Storms-Ecomomic And Public Health Impact In The USA."
author:
- affiliation: iNTELLIGENTIANALYTICs
  email: patrickleugue@gmail.com
  name: Patrick Leugue
date: "Monday, August 19, 2014"
output: pdf_document
bibliography: sigproc.bib
subtitle: An exploration of NOAA storm data for the cost analysis of the differents
  types of storms.
abstract: "As early as 1826, data on severe weather occurences has been gathered and
  recorded. That information gathering task has been continued by the US National
  Oceanographic Atmospheric Agency (NOOA,) which uses cutting edge technology to collects,
  process, and save data about storms, from thousands of sensors disseminated all
  over the US.  All the data is made available to the broader public via it's website.
  \n\nThe data reveals that Tornadoes, Thunderstorm Winds and Flood have the greatest
  economic impact with approximately 10 Billions in property and crop damages per
  year. They represents an equally important public health treat with an estimated
  6000 peoples killed or injured every year. The findinds in this paper were obtained
  by exploratory analyses of NOAA's Storm information from 1950 to November 2011.\n"
---



# Introduction 
The United States are affected every year by natural disasters caused by storms. The US goverment spends approximately 2 billions dollars yearly to support and indemnify the victims [@meier2012].  In 2005 alone, damages from storms were evaluated at 2.5 billions dollars[@meier2012] and 2500 fatalities were officially recorded.

Every year, as it has been since 1826, NOAA(National Oceanographic Athmospheric Agency) collect and compiles data about storms-related occurences on the US soil. The data includes an estimation of property and crop damages, as well as a count of fatalities and injuries per event. All events are categorized by their type and additional location information is provided. 

To determine what type of storm event has the greatest economical and public health impact, storm data from 1950 to November 2011 is obtained from NOAA, and Exploratory analysis is conducted on the data.

# Data Processing
Data analysis and processing is conducted using the free and open source R statistical analysis toolset.The environment consist of RStudio Version 0.98.953 and the following R parameters:

```r
opts_chunk$set(echo=TRUE, cache=TRUE)
R.version()
```

```
## Error: could not find function "R.version"
```

To answer the two questions about the effect of storm events on public health and the economy, storm data from 1950 to November 2011 is obtained from [here](https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2FStormData.csv.bz2) 

```r
#  Link to the compressed data file on website
#fileURL <- "https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2FStormData.csv.bz2"
#download.file(fileURL, destfile="storm.bz2")
```
decompressed into the current folder,

```r
#require(R.utils)
#bunzip2("./storm.bz2")
```
and the raw data is imported into the R environment

```r
#rawdata <- read.csv("repdata-data-StormData.csv")
```

A decription of imported data is available in the [Storm Data Documentation](https://d396qusza40orc.cloudfront.net/repdata%2Fpeer2_doc%2Fpd01016005curr.pdf). 
A peek at the data structure should help identify all the attributes described in the document above.

```r
#str(rawdata)
```


The raw data can be subsetted to contain only attributes that matter: Event type, Property damage, Crop Damage, Property damage Exponent, Crop damage Exponent


# Results
Nullam semper imperdiet orci, at lacinia est aliquet et. Sed justo nibh, aliquet et velit at, pharetra consequat velit. Nullam nec ligula sagittis, adipiscing nisl sed, varius massa. Mauris quam ante, aliquet a nunc et, faucibus imperdiet libero. Suspendisse odio tortor, bibendum vel semper sit amet, euismod ac ante. Nunc nec dignissim turpis, ac blandit massa. Donec auctor massa ac vestibulum aliquam. Fusce auctor dictum lobortis. Vivamus tortor augue, convallis quis augue sit amet, laoreet tristique quam. Donec id volutpat orci. Suspendisse at mi vel elit accumsan porta ac ut diam. Nulla ut dapibus quam.

Sed est odio, ornare in rutrum et, dapibus in urna. Suspendisse varius massa in ipsum placerat, quis tristique magna consequat. Suspendisse non convallis augue. Quisque fermentum justo et lorem volutpat euismod. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Morbi sagittis interdum justo, eu consequat nisi convallis in. Sed tincidunt risus id lacinia ultrices. Phasellus ac ligula sed mi mattis lacinia ac non felis. Etiam at dui tellus.


# Conclusion
Duis nec purus sed neque porttitor tincidunt vitae quis augue. Donec porttitor aliquam ante, nec convallis nisl ornare eu. Morbi ut purus et justo commodo dignissim et nec nisl. Donec imperdiet tellus dolor, vel dignissim risus venenatis eu. Aliquam tempor imperdiet massa, nec fermentum tellus sollicitudin vulputate. Integer posuere porttitor pharetra. Praesent vehicula elementum diam a suscipit. Morbi viverra velit eget placerat pellentesque. Nunc congue augue non nisi ultrices tempor.

# References

---
references:
- id: meier2012
  title: Professinal Android 4 Application Development
  author: 
  - family: Meier
    given: Reto
  type: book
  publisher: John Wiley & Sons, Inc.
  issued:
    year: 2012
    month: 5
- id: fenner2012a
  title: One-click science marketing
  author:
  - family: Fenner
    given: Martin
  container-title: Nature Materials
  volume: 11
  URL: 'http://dx.doi.org/10.1038/nmat3283'
  DOI: 10.1038/nmat3283
  issue: 4
  publisher: Nature Publishing Group
  page: 261-263
  type: article-journal
  issued:
    year: 2012
    month: 3
...

