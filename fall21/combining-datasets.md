# Examples of Combining Datasets in Visualizations

I've recently come across a couple nice examples of combining datasets in visualizations. I'll show them here along with previous examples that I've shown.

## US COVID Case Rates and US County Demographics

<img src="imgs/US-covid-metro.png" height="400"/>

I saw this visualization through a [tweet by @agsciencewriter](https://twitter.com/agsciencewriter/status/1467521843162750976).  It's based on data from the CDC and can be reproduced at [Trends in COVID-19 Cases and Deaths in the United States, by County-level Population Factors](https://covid.cdc.gov/covid-data-tracker/#pop-factors_7daynewcases).

Read the "Footnotes" section to understand where all of the data comes from and how it's calculated.

Data combinations:
* COVID case rate by county
* US county metro vs. non-metro classification, from https://www.cdc.gov/nchs/data_access/urban_rural.htm

## Missouri Mask Mandates and COVID Case Rates

<img src="imgs/missouri-mask-cases.png" height="400"/>

This visualization comes from an article in the *Missouri Independent* news, ["Missouri health department found mask mandates work, but didn’t make findings public"](https://missouriindependent.com/2021/12/01/missouri-health-department-found-mask-mandates-work-but-didnt-make-findings-public/) ([larger version w/tooltips](https://datawrapper.dwcdn.net/gSx9f/4/))

It splits out the case rates in St. Louis, St. Louis County, Kansas City and Jackson County (all with mask mandates) from the rest of the state. They found that "jurisdictions with mask mandates averaged 15.8 cases per day for every 100,000 residents, compared to 21.7 in unmasked communities."

Data combinations:
* COVID case data by county 
* Set of counties that had mask mandates
* Dates of significant events around Delta, case surges, and mask mandates

## California Spending on Universities and Dept of Corrections

<img src="imgs/california-univ-corrections.jpeg" height="400"/>

"This shocking graph is from a new @SREJournal article by Hamilton, Nielsen, and Larma. Over the past 50 years, California state budget priorities for university and incarceration have dramatically reversed. As HE funding declines, minority students suffer."  
Source: https://twitter.com/nathanihoff/status/1465454549385105410

Data combinations:
* Amount of state funding for University of California and California State University systems
* Amount of state funding for corrections (jails and prisons)

Note that the raw amounts aren't used, but rather the share of the state budget those amounts represent.  This allows the lines to be drawn on the same chart with the same scale.

## Louisiana COVID Cases, Deaths, Vaccinations

<img src="imgs/louisiana-covid.png" height="400"/>

This visualization comes from an article in *The Times-Picayune | The New Orleans Advocate*, ["Louisiana COVID numbers: Data on cases, deaths, hospitalizations, vaccines"](https://www.nola.com/news/coronavirus/article_7cb2af1c-6414-11ea-b729-93612370dd94.html) ([archived version, Sep 2021](http://web.archive.org/web/20210927011921/https://www.nola.com/news/coronavirus/article_7cb2af1c-6414-11ea-b729-93612370dd94.html))

Data combinations:
* COVID cases, 7-day average
* COVID hospitalizations
* COVID deaths
* COVID vaccination percentages
* key dates related to mask mandates, Delta variant, and vaccine availability

## US Poverty Rate, IRS Auditing Rate, and 2016 Political Affiliation

<img src="imgs/Poverty-Audit-Rate2.png" height="400"/>

This visualization comes from ["Geographic Distribution of IRS Auditing Rates"](https://policyviz.com/2019/05/02/geographic-distribution-of-irs-auditing-rates/) in [PolicyViz.com](https://policyviz.com). 

Data combinations:
* US poverty rate by county, from https://factfinder.census.gov/faces/tableservices/jsf/pages/productview.xhtml?pid=ACS_17_1YR_S1903&prodType=table
* IRS auditing rate by county, from https://www.propublica.org/datastore/dataset/irs-audit-rates-by-county
* Voting in the 2016 US Presidential Election, from https://github.com/tonmcg
