# ChE 2410 Project 1: How transportation usage and population density interact with covid infection rates.

Abstract: in 2021 Americans slowly started using public transportation again after the dropoff during the early COVID period. Given apparent shared space occuring in public transportation, was the rate of public transportation usage a factor in COVID case rates in 2021? This data analysis looks into answering this question using existing public datasets to generate vizualizations of what relationships may exist between different measurements of American counties. 

No significant relationship was found between whether a county had significant public transportation usage and their according case count in 2021. Future observations should look into more specific slices such as particular metropolitan areas or specific time periods.

Code runs normally except for 1_ and 4_ which reference https://github.com/nytimes/covid-19-data the us-counties 2021 file. Everything else is created and referenced internally. Code runs on python version 3.9.12, seems to behave differently if 3.1 is used.

Note: background on images is transparent, use non-dark themes to see the graphs below.

<img src="./casesperpophist.png" width="400" />

This is a histogram of total cases per capita. Further outliers are omitted with even higher total case counts. Total cases per capita is across a year, corresponding average cases per capita would be the total divided by number of reported cases, 365.

<img src="./cases_vs_logptu_densitycolored.png" width="400" />

Log10 of public transportation usage versus cases per capita, one dot is a county. Colored based on log10 of population density.

<img src='./linmodel.png' width='400'>

Previous graph with linear and average solutions. Both carry high SSEs indicating poor fits; a relationship between these data is not visible.

<img src='./nonlinmodel.png' width='400'>

Log10 of public transportation usage versus log10 of population density. Nonlinear, linear, and average solutions displayed. A poor fit to noisy data, but a relationship was nonetheless described.
