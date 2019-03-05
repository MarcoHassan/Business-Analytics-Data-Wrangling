# Business Analytics Project

This code was operated on a vast dataset of aggregated data. The code abstract from statistical evalutation and focuses on descriptive statistics, data wrangling through **SQL and dplyr queries**.

SQL queries were integrated in the R code through the **sqldf package** that allows to make use of sql queries to operate on data frames in R. Important to notice, is the difference with the **DBI package**. Where the latter offers the option to connect to RDMS the first just allows to run SQL queries on local mode.

Moreover the code contains the mapping of the descriptive statistics by country plotted on the classical merchator map.

### Mapping Strategy

In order to do that I downloaded the merchator map and the country specific centroid coordinates through the **getMap** function of the **rworldmap** package. I joined the new obtained dataset with the dataset of interest based of the country code. This result in an integrated dataset from which I could plot descriptive statistics of interest on the merchator map.

### Mapping example

![image](https://user-images.githubusercontent.com/42472072/52440030-c4613500-2b25-11e9-8b1e-ba8d95066815.png)
