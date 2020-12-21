*This is the public posting of the assignment. See Blackboard for the invite link to make your submission in your own repository in the class organization*

# Homework 7: Generating Questions from Real-World Data

**Due:** Tuesday, December 1, 2020 by 11:59pm

HW7 and HW8 are the last two assignments of the semester.  In HW7 (this assignment), you will use EDA techniques to generate questions from a dataset(s) and propose charts to address those questions.  In HW8, you will take one of the proposed charts from HW7 and refine it based on storytelling/data journalism techniques so that it is suitable for presentation.

## Assignment

Use the EDA process to explore a dataset or datasets of your choice.  Through this process, you should generate at least 2 detailed questions that can be most effectively answered through visualization (rather than just directly reporting the results).  Sketch (on paper) or draft (using the tool of your choice) charts that could address and answer those questions.

Often the most interesting questions and analysis come from the combination of multiple datasets, so consider how you might ask questions of your initial dataset that might require obtaining an additional dataset.

The Data Sources section below contains links to several public data sources. Be careful about the size of the dataset. You probably want on the order of 100s-1000s of items rather than millions.  

Since you can ask better questions about data you know about, you should pick a dataset that you have some knowledge about or that you are personally interested in learning more about.  *For your own benefit, you should choose your dataset no later than Tue, Nov 17.*

I *strongly encourage* you to discuss your topic, datasets, questions, and proposed charts with me well in advance of the deadline.  This can be done via email or via Zoom (either during office hours or with a separately scheduled appointment).

## Report

Your report is an important part of this assignment. I expect your report to include your name, CS625-HW7, date, and appropriate headings and Markdown markup for clarity and neatness. You will lose points if there are many spelling or grammatical errors. 

Your report should contain the following information:
* description of your dataset (including a link to the original source of the data)
* description of your EDA process - explain the initial questions you asked, describe any statistics or charts created to initially explore the data, and describe how you generated additional questions
* final detailed questions that you arrived at
* images of your sketch or draft charts
* explanations of the charts and how they will be used to answer the detailed questions

If you use R, any code needed to document your EDA process should be runnable and embedded in your RMarkdown report. Make sure to 'Knit' your report to produce Markdown suitable for Github and commit both the .Rmd and .md files to your repo. 

If you use Vega-Lite, your report must include a link to the Observable notebook that contains your Vega-Lite code and charts.

As always, you must include a section titled "References", including links to any examples that you used in completing this assignment.

## Data Sources

This is just a sample of the various public datasets that are freely available online.

**Public Data Collections**
* ProPublica's data store - https://www.propublica.org/datastore/datasets
* fivethirtyeight.com datasets - https://data.fivethirtyeight.com
* BuzzFeedNews datasets - https://github.com/BuzzFeedNews/everything

**COVID-19 data**
* Virginia Department of Health - https://www.vdh.virginia.gov/coronavirus/
* COVID Tracking Project - https://covidtracking.com
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
Make sure that you have committed and pushed your local repo to GitHub.  Include "Ready to grade @weiglemc" in your final commit message. 

Submit the URL of your report in Blackboard:
* Click on HW7 under Assignments in Blackboard
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your `report.md` file into the edit box (should be something like https<nolink>://github.com/cs625-datavis-fall20/hw7-questions-*username*/blob/master/report.md)
* Make sure to "Submit" your assignment.
