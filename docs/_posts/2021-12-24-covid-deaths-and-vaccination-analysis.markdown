---
layout: post
title:  "Covid Deaths and Vaccination Analysis"
excerpt: "This analysis of vaccinated deaths is done to determine and rank the effectiveness of the vaccine brands taken by Malaysians. In order to have a fair representation of the vaccine effectiveness against COVID-19, individuals with commorbidities and those with less than 2 vaccination doses are removed."
date:   2021-12-24 15:46:34 +0800
categories: covid-19
---

## About

This analysis of vaccinated deaths is done to determine and rank the effectiveness of the vaccine brands taken by Malaysians.

From the original source deaths data published by the Ministry of Health - [link here](https://github.com/MoH-Malaysia/covid19-public). In order to have a fair representation of the vaccine effectiveness against COVID-19, individuals with commorbidities and those with less than 2 vaccination doses are removed.

The entire analysis was done in jupyter notebook and written in python - [source code](https://github.com/marksia/covid_deaths_and_vaccination/blob/main/Covid%20Deaths%20by%20Vaccine.ipynb). HTML file available [here](https://github.com/marksia/covid_deaths_and_vaccination/blob/main/Covid%20Deaths%20by%20Vaccine.html).

&nbsp;

## Main Findings

- Total deaths as at 24th December 2021: `31,265`
- Individuals with commorbidities: `24,201`
- Total deaths after removing commorbidities: `7,064`
- Individuals with less than 2 vaccine doses: `6,459`
- Total deaths after removing commorbidities and those with 1 dose of vaccine or less: `605`

Out of the 605 remaining rows of data, the vaccine types breakdown are as follows:

**By Count:**

![vaccinated-deaths-by-brand](/assets/images/vaccinated-deaths-by-brand.png)

**By Percentage:**

![vaccinated-deaths-by-brand-percentage](/assets/images/vaccinated-deaths-by-brand-percentage.png)

**By Age Grouping**:
![vaccinated-deaths-by-brand-and-age-groups](/assets/images/vaccinated-deaths-by-brand-and-age-groups.png)

As observed with the preceding bar charts, Sinovac vaccinated individuals has the highest proportion of cases, followed by Pfizer and AstraZeneca. This trend is also consistent across the different age groups.

The total vaccine brands issued all time (Data from [COVIDNOW](https://covidnow.moh.gov.my/vaccinations) as at 24th December 2021) are as follows:

- Cansino: `0.4%`
- AstraZeneca: `7.3%`
- Sinovac: `36.6%`
- Pfizer: `55.7%`

**As you can see, the proportion of vaccinated deaths as compared to the proportions of vaccines issued are not the same. There are more Pfizer vaccines given out over time as compared to Sinovac, but the proportion of vaccinated deaths are higher with Sinovac as compared to Pfizer. AstraZeneca has the best statistics out of the three brands.**

&nbsp;

## Gender distributions

Male vs Female Covid Death rates - original data without removing commorbidities or unvaccinated.

- Male Percentage of Death: `57.44%`
- Female Percentage of Death: `42.56%`

Male vs Female Covid Death rates - 2 vaccine doses, removed commorbidities

- Male Percentage of Death: `66.12%`
- Female Percentage of Death: `33.88%`

**Male seems to have a higher chance of death by covid with or without vaccinations.**

&nbsp;

## Some Good News

For those that have taken 2 vaccines and do not have commorbidities:

- Sinovac: you have `1.56%` chance of death by covid
- Pfizer: you have `0.32%` of death by covid
- AstraZeneca: you have `0.04%` of death by covid

**Get vaccinated and stay healthy** 🙂

&nbsp;

## Disclaimer

The findings shown in this post is not any form of advice. The analysis is only as accurate as the data provided - read [Garbage in, garbage out](https://en.wikipedia.org/wiki/Garbage_in,_garbage_out). The analysis is done based on historical data and is no guarantee of future results and effectiveness against new variants. The long term effects of different vaccines are not known. You can view the entire source code and data I have used to come out with the analysis and make your own conclusions.

&nbsp;

## Links

- [Full Source Code Repo](https://github.com/marksia/covid_deaths_and_vaccination)
- [Open data on COVID-19 in Malaysia](https://github.com/MoH-Malaysia/covid19-public)
