## Overview
The purpose of this project is to gain familiarity with Apache Spark through its Python implementation, PySpark. Spark is more appropriate for processing large amounts of data as it does not load it into memory like R's default implementation or Python's Pandas. Spark is also able to split its work into parrallel processes.

The data set used here is the Public Use Microdata Sample (PUMS) provided by the US Census Bureau. It contains a sample from the US Census with data points such as age, race, income, home value, and other data.
- [PUMS Survey Data](https://catalog.data.gov/dataset/2006-2008-american-community-survey-3-year-pums-population-file)

This analysis is to find simple relationships in the data. In this case, I compared the income of minorities to white people and ranked the US states and territories based off of the discrepency found.
* [Demonstration Video](http://youtube.link.goes.here)

## Data Analysis Results
I had a few questions I wanted to explore in this dataset. I believed there was likely some discrepency between income for minority groups. My two main questions were:
- Is there a significant difference in income between white people and minority groups?
- If so, how does this vary accross states?

My findings did show that there is a significant difference in the average income between the two groups. Although this may be in part due to discrimination, this would need to proven with more analysis.
I was also able to rank states in the US by the discrepency found in each one. Again, more analysis on this dataset will need to be done to confirm the results are not skewed.
**Least discrepency**:
![](/Images/top_five.png)
**Most discrepency**:
![](/Images/bottom_five.png)
## Development Environment
For this project I used Python and the PySpark package. To use PySpark, you'll need to install Java and Scala. The code was written using VS Code.
## Useful Websites
Documentation for how to use PySpark (I used the Spark SQL API in Python, but you can use the others as well).

I also followed a tutorial from freeCodeCamp.org to learn the basics. I only needed to watch the first half, but there is more if you need it.
* [Apache Spark API Reference](https://spark.apache.org/docs/latest/api/python/reference/index.html)

* [freeCodeCamp.org Tutorial (on YouTube)](https://youtu.be/_C8kWso4ne4)
## Future Work
To make this analysis more robust, I need to do a few things.
* Clean the data. I did not spend much time looking at the data in the columns I used, so there may be values that are throwing skewing the results.
* Fix median wages. I also generated a chart to look at the median wages of a household, but the numbers seemed off. I need to verify their accuracy.
* Add a check for immigration status. I think immigration status could change how much people make. I would like to separate that group in the future as a control.
* General: investigate other reasons for the difference in yearly wages (e.g. wages are closer in one state because everyone is paid worse there rather than there being less discrimination).