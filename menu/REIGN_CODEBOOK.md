---
title: "Rulers, Elections and Irregular Governance Dataset (REIGN) Codebook"
author: "Clayton Besaw (cbesaw@oneearthfuture.org)"
date: 'June 3, 2020'
output: html_document
---

```{R include=FALSE}
df <- read.csv("D:/Dropbox/OEF/coupcast-reign misc/REIGN Translate/REIGN_2020_6.csv")
```

The Rulers, Elections and Irregular Governance Dataset (REIGN) collects data concerning the political leadership, regime characteristics and electoral outcomes for every country around the globe since January 1950. REIGN is measured at the country-leader-month level and contains `r nrow(df)` observations as of `r format(Sys.Date(), "%B %d, %Y")`. 

REIGN is updated monthly with public updates released typically on the first Tuesday of every new month. This codebook serves as a living document for navigating REIGN measurements and is subsequently updated each month alongside the new REIGN data updates. 

REIGN was originally created and curated by [Curtis Bell](https://scholar.google.com/citations?user=WKi4SYIAAAAJ&hl=en), who has since moved on to lead his new research and policy program called [Stable Seas](https://stableseas.org/). REIGN is now curated and maintained by the One Earth Future Political Forecasting program with on-going support and improvements planned for a long-term lifespan. 

REIGN builds off a number of previous data projects alongside its own original data collection. For more details on the sources that underpin REIGN and similarities/differences, please consult our extended technical notes [here](https://cdn.rawgit.com/OEFDataScience/REIGN.github.io/gh-pages/documents/reign_notes.pdf)

# CODEBOOK AND MEASURE DESCRIPTIONS
## Country and Time Measures

* **ccode**: ccode is a one to three digit number that uniquely identifies each of the 201 countires included in the dataset. These numbers align with those used by other large cross-national datsets, including Correlates of War. The ccode is most useful for merging REIGN with other datasets that also share a cow country code. 

* **country**: country provides the full colloquial name for the country observed in the row. Not all country names are full legally recognized country names. 

* **year**: year is the calendar year, ranging from 1950 to `r max(df$year)`. 

* **month**: month identifies the month number ranging from 1 (January) to 12 (December)

## Political Leader Characteristics

* **leader**: Provides the de factor leader's name. Note: Leader names are no unique, so any sorting or panel identification should be done using country and time characteristics to identify unique leader periods. 

```{r include=FALSE, echo = FALSE}
library(summarytools)

```

* **elected**: elected is a binary measurement that indicates whether the de facto leader had previously been elected (1) or not (0) to their respective office. Individual leaders can have tenure periods in which they were both not-elected and elected. This happens when a leader comes to power through a non-electoral mechanism (resignation, death of incumbent, coup, etc) and is eventually elected later on through a national election event. 
`r print(freq(df$elected), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **age**: age is an approximation of the leader's age calculated by subtracting the leader's birth year from the current year. This does not account for a leader's specific birth date. It takes the same value for each month in a calendar year. In the rare event that a leader's birth date is not known, we estimate it using peer leader multiple imputation using a Random Forest algorithm. 
`r print(descr(df$age, stats = c("mean", "sd", "min", "max", "N.Valid")), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **male**: male is a dummy variable to account for the sex of the de facto leader. This measure equals 1 if a leader is male and 0 if the leader is female. 
`r print(freq(df$male), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **militarycareer**: military career is equal to 1 if the leader's primary career and/or source of authority comes from their career in the military, police force or defense ministry. Previous service is not necessarily sufficient for coding this. Rather, this designation is reserved for those whose primary affiliation prior to taking power can be described by a long-term career in the previous three categories
`r print(freq(df$militarycareer), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **tenure_months**: tenure_months counts the number of months that a leader has been in power during their current tenure period. Typically, a leader's inaguaral month will start at 1 and continue until resetting during a leader change. However, some leaders in 1950 will have tenure months that reflect their previous tenure before January 1950. 
`r print(descr(df$tenure_month, stats = c("mean", "sd", "min", "max", "N.Valid")), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

## Elections and Leader Change

* **anticipation**: anticpation is a dummy variable that equals 1 if there is an election for the de facto leadership position coming within the next six-months. **All election anticipation measures are constructed using official announcement dates and/or constitutional deadlines/scheduling when available.** 
`r print(freq(df$anticipation), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **ref_ant**: ref_ant is a dummy variable that equals 1 if there is a constitutional referendum coming within the next six-months. 
`r print(freq(df$ref_ant), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **leg_ant**: leg_ant is a dummy variable that equals 1 if there is a legislative election to determine the de facto leader coming within the next six-months. 
`r print(freq(df$leg_ant), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **exec_ant**: ref_ant is a dummy variable that equals 1 if there is an executive election to determine the de facto leader coming within the next six-months. 
`r print(freq(df$exec_ant), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **irreg_lead_ant**: irreg_lead_ant is a dummy variable that equals 1 if an irregular election to determine the de facto leader is expected within the next six months. 
`r print(freq(df$irreg_lead_ant), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **election_now**: election_now is a dummy variable that equals 1 if there is an election for the de facto leadership position taking place in that country-month. 
`r print(freq(df$election_now), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **delayed**: delayed is a dummy variable that equals 1 if a previously scheduled/expected election is cancelled by choice or through exogenous factors (e.g. regime change).
`r print(freq(df$delayed), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **lastelection**: lastelection is an inverted decay function that measures the time since the last election for the de facto leadership position within the country. The measure is 0 when election_now equals 1. The number grows following the election until it resets at the next election. Higher values indicate longer periods since the last election.
`r print(descr(df$lastelection, stats = c("mean", "sd", "min", "max", "N.Valid")), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **election_recent**: election_recent is a dummy variable that equals 1 if there is an election for the de facto leadership position that took place in the previous six months. 
`r print(freq(df$election_recent), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **leg_recent**: leg_recent is a dummy variable that equals 1 if there is a legislative election took place in the previous six months. 
`r print(freq(df$leg_recent), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **exec_recent**: exec_recent is a dummy variable that equals 1 if there is an executive election took place in the previous six months. 
`r print(freq(df$exec_recent), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **ref_recent**: ref_recent is a dummy variable that equals 1 if there is a constitutional referendum took place in the previous six months. 
`r print(freq(df$ref_recent), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **direct_recent**: direct_recent is a dummy variable that equals 1 if a direct (popular) election took place in the previous six months. 
`r print(freq(df$direct_recent), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **indirect_recent**: indirect_recent is a dummy variable that equals 1 if an indirect (elite) election took place in the previous six months. 
`r print(freq(df$indirect_recent), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **lead_recent**: lead_recent is a dummy variable that equals 1 if an electoral opportunity to change leadership took place in the previous six months.
`r print(freq(df$lead_recent), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **victory_recent**: victory_recent is a dummy variable that equals 1 if an incumbent political party/leader won an election in the previous six months.
`r print(freq(df$victory_recent), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **defeat_recent**: defeat_recent is a dummy variable that equals 1 if an incumbent political party/leader won an election in the previous six months.
`r print(freq(df$defeat_recent), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **change_recent**: change_recent is a dummy variable that equals 1 if the de facto leader changed due to an election in the previous six months. (note: the incumbent party can win and leadership change can still happen if the specific leader changes).
`r print(freq(df$change_recent), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **nochange_recent**: nochange_recent is a dummy variable that equals 1 if the de facto leader did not change following an election in the previous six months. 
`r print(freq(df$nochange_recent), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

## Country Characteristics

* **government**: government corresponds to the regime type of the country during the observed country-month. Government categories can correspond to 16 regime types that capture democracies, non-democracies and interim governments. These categories are: 1. presidential democracy, 2. parliamentary democracy, 3. personalist system, 4. monarchy, 5. single-party system, 6. oligarchy, 7. party-personalist hybrid, 8. military junta, 9. indirect military junta, 10. personalist-military hybrid, 11. party-military hybrid, 12. party-personalist-military hybrid, 13. warlordism, 14. foreign-occupation, 15. civilian provisional government, 16. military provisional government.
`r print(freq(df$government), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **prev_conflict**: prev_conflict is equal to the number of on-going violent civil conflicts occuring somewhere in the country during the previous month. The measure ranges from 0 (no previous conflicts) to any positive integer indicating exisiting conflicts. As of `r format(Sys.Date(), "%B %d, %Y")` the maximum number of civil conflicts a country has faced is `r max(df$prev_conflict)`. 
`r print(freq(df$prev_conflict), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **precip**: precip measures the Standardized Percipitation Index (SPI) for each country month. You can interpet precip like a Z-score. Values of 0 correspond to historically average levels of rainfall for that country-month. Positive values above 0 indicate more rainfall than historically expected, with values greater than 1.96 generally corresponding to a statistically significant increase in rainfall. Conversely, you can interpret negative values as indicating less than expected rainfall. The underlying data comes from [NOAA's PREC/L](https://psl.noaa.gov/data/gridded/data.precl.html) observation data, with future months forecasted by using country-specific optimized ARIMA models. As of `r format(Sys.Date(), "%B %d, %Y")`, ground-truth data ends at *April 2020*, with the forecast taking place from *May 2020* to *December 2020*. 
`r print(descr(df$precip, stats = c("mean", "sd", "min", "max", "N.Valid")), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **couprisk**: couprisk is an estimated probability of the risk of a military coup attempt taking place in the country-month. couprisk is estimated by using machine-learning classification and a stacking algorithm that combines the individual predictions of a (a) random forest algorithm, (b) logistic regression model and (c) linear probability regression model. A Generalized estimating equation is then used to combine the weighted probabilites of each previous model to take advantage of each model's strengths while minimizing poor predictions. Model training is performed through rolling-origin cross-validation using 1950 - 1974 as the initial training window. As such, couprisk estimates only begin in January, 1975 until `r format(Sys.Date(), "%B, %Y")`. 
`r print(descr(df$couprisk, stats = c("mean", "sd", "min", "max", "N.Valid")), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`

* **pctile_risk**: pctile_risk corresponds to the percentile risk for each country's estimated risk of a military coup attempt that month. This is a standard risk percentile that ranges from 0 (risk lower than 100% of countries that month) to 1 (risk higher than 100% of all other countries that month). Since our couprisk measure is somewhat conservative, pctile_risk provides a way to examine more coup risk in relation to all other countries that month.
`r print(descr(df$pctile_risk, stats = c("mean", "sd", "min", "max", "N.Valid")), method = "render", table.classes = 'st-small', report.nas = FALSE, headings = FALSE)`
