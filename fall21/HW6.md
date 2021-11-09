*This is the public posting of the assignment. See Blackboard for the invite link to make your submission in your own repository in the class organization*

# Homework 6: Project - Initial Dataset Exploration
**Due:** November 16, 2021 by 11:59pm

HWs 6-8 are the final assignments of the semester and will build up to a final visualization.  The end goal is to produce a static *explanatory* visualization that reveals some interesting relationship between two datasets.  (I highlighted 3 of last year's projects in a [blog post earlier this year](https://ws-dl.blogspot.com/2021/04/2021-04-05-data-visualization-fall-2020.html), though note that they had a slightly different assignment.)

The table below provides an overview of the three assignments.

|assignment|main tasks|due date|
|---|---|---|
|HW 6|choose your main dataset, start the EDA process|Tue, Nov 16|
|HW 7|gather the 2nd dataset, generate specific questions, sketch proposed charts|Tue, Nov 30|
|HW 8|fully develop the final chart|Sun, Dec 12|

I strongly encourage you to discuss your topic, datasets, questions, and proposed charts with me well in advance of the deadlines. I want to give you feedback as you work through this process. This can be done via email or via Zoom (either during office hours or with a separately scheduled appointment).

## Assignment

You will write a report in Markdown that describes how you completed the following two steps.

### Step 1: Choose a Dataset

Since you can ask better questions about data you know about, you should pick a dataset that you have some knowledge about or that you are personally interested in learning more about. 

The [Data Sources section](#data-sources) below contains links to several public data sources. Be careful about the size of the dataset. You probably want on the order of 100s-1000s of items rather than millions.

In your report, talk about your interest in the topic and link to your data source. Note that if you found the dataset on Kaggle, I'd also like a link to the original source of the data, if available.

### Step 2: Start the EDA Process

Use the EDA process to start exploring your dataset. Review the [Exploratory Data Analysis chapter](https://r4ds.had.co.nz/exploratory-data-analysis.html) from *R for Data Science* as you work through this step.  Often the most interesting questions and analysis come from the combination of multiple datasets, so your questions should be of the type that could be addressed by combining your main dataset with another dataset. (At this step, you do *not* need to obtain an additional dataset -- that will be done in HW7.) 
> Example: Do COVID infection rates in Virginia health districts change with the vaccination rate in the district?  This would require combining the infection data with vaccination and population data for each district.

Generate at least 2 questions that can be most effectively answered through visualization (rather than just directly reporting the results).  These questions should be the result of your initial EDA process.  Note that in HW7 you will have the opportunity to further develop the questions to explore in your project.

In your report, describe your EDA process.  Talk about how you moved from initial analysis and questions about the data to the final questions that you submit.
You may generate overview or distribution charts as you work through the EDA process. Your report should describe any data manipulation and include any analysis charts that you developed as part of this initial EDA process.  You may use any tool of your choice for this step.

As always, your report must include a section titled "References", including links to any examples or references that you used in completing this assignment.

### Data Sources

This is just a sample of the various public datasets that are freely available online.

**Public Data Collections**
* Teaching Datasets - https://observablehq.com/@mkfreeman/teaching-datasets
* ProPublica's data store - https://www.propublica.org/datastore/datasets
* fivethirtyeight.com datasets - https://data.fivethirtyeight.com
* BuzzFeedNews datasets - https://github.com/BuzzFeedNews/everything

**COVID-19 data**
* Virginia Department of Health - https://www.vdh.virginia.gov/coronavirus/  (click the plus sign next to "To download COVID-19 data sets, click below." to see the datasets)
* Federal COVID data sources, compiled by The COVID Tracking Project - https://covidtracking.com/analysis-updates/federal-covid-data-101-how-to-find-data
* Coronavirus (Covid-19) Data in the United States, *New York Times* - https://github.com/nytimes/covid-19-data
* State-level social distancing policies in response to the 2019 novel coronavirus in the US - https://github.com/COVID19StatePolicy/SocialDistancing

**Government data**
* US Government data - https://www.data.gov
* US employment - https://www.bls.gov/data/
* US demographics - https://www.census.gov/data.html
* FBI Crime Data - https://www.fbi.gov/services/cjis/ucr/
* US Centers for Disease Control (CDC) - https://www.cdc.gov/datastatistics/index.html
* UK Government data - https://data.gov.uk
* World Bank data - https://databank.worldbank.org/data/home.aspx

**Weather/Climate**
* water levels - https://tidesandcurrents.noaa.gov
* Hampton Roads tide predictions - http://coastalslr.blogspot.com/2017/12/hampton-roads-tide-predictions.html
* climate - https://www.ncdc.noaa.gov/cdo-web/datatools
* hurricanes - http://www.nhc.noaa.gov/analysis_tools.php
* other weather events over time - https://www.ncdc.noaa.gov/data-access

**TV News archive**
* Internet Archive's TV News Archive - https://archive.org/details/tv
  * intro - https://blog.archive.org/2014/04/01/tv-news-intro/
  * example uses - http://blog.archive.org/2017/12/27/tv-news-record-the-year-in-tv-news-visualizations/

## Submission
Make sure that you have committed and pushed your local repo to GitHub.  Include "Ready to grade @weiglemc @javedulferdous" in your final commit message. 

Submit the URL of your report in Blackboard:
* Click on HW6 under Assignments in Blackboard
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your `report.md` file into the edit box (should be something like https<nolink>://github.com/odu-cs625-datavis/fall21-hw6-*username*/blob/master/report.md)
* Make sure to "Submit" your assignment.
