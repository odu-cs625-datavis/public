*This is the public posting of the assignment. See Blackboard for the invite link to make your submission in your own repository in the class organization*

# Homework 3: Arrange Tables 

**Due:** Tuesday, October 6, 2020 by 11:59pm 

The goal of this assignment is to practice choosing and implementing approriate chart idioms based on given data and questions.

## Dataset
We are going to examine the [Virginia Department of Health's COVID-19 Dataset](https://www.vdh.virginia.gov/coronavirus/). The dataset, [VDH-COVID-19-PublicUseDataset-Tests_by-LabReportDate](https://data.virginia.gov/Government/VDH-COVID-19-PublicUseDataset-Tests_by-LabReportDa/3u5k-c2gr), has been made available through the [Virginia Open Data Portal](https://data.virginia.gov).  *Click the Export button on the dataset page to download the CSV.*

> This data set includes the number of COVID-19 testing encounters and positive tests for PCR tests and all test types for each health district in Virginia by lab report date. This data set was first published on May 15, 2020. When you download the data set, the dates will be sorted in ascending order, meaning that the earliest date will be at the top. To see data for the most recent date, please scroll down to the bottom of the data set.

We will also be considering the survey *The New York Times* conducted July 2-14 regarding mask usage. The data is available in the [Mask-Wearing Survey Data](https://github.com/nytimes/covid-19-data/tree/master/mask-use) GitHub repo.  This data is organized by [county-level FIPS codes](https://www.nrcs.usda.gov/wps/portal/nrcs/detail/?cid=nrcs143_013697).  *There's a link to the Raw CSV in the repo's README file.*

> This data comes from a large number of interviews conducted online by the global data and survey firm Dynata at the request of The New York Times. The firm asked a question about mask use to obtain 250,000 survey responses between July 2 and July 14, enough data to provide estimates more detailed than the state level. ... Specifically, each participant was asked: How often do you wear a mask in public when you expect to be within six feet of another person?


## Assignment

Explore the datasets and create a chart for each of the following questions (VDH = Virginia Dept of Health, NYT = New York Times mask survey):

1. [VDH] How does the percentage of positive PCR tests over time compare for Norfolk, Chesapeake, and Virginia Beach?  
    * If you don't live in one of those cities, feel free to add your city or health district.
    * You can compute and show the 7-day [moving average](https://en.wikipedia.org/wiki/Moving_average) instead of the daily percentage, but you are not required to.

1. [VDH] For each health district, what percentage of the total tests given were PCR tests?

1. [VDH, NYT] Was there a correlation between the percentage positive PCR tests averaged over July 16-28 (two weeks after the mask survey) and the estimated share of residents that answered "Frequently" or "Always" to the question of mask usage?  
     * Show this for the following 15 health districts only: Norfolk, Virginia Beach, Chesapeake, Portsmouth, Hampton, Western Tidewater, Peninsula, Fairfax, Arlington, Prince William, Richmond, Henrico, Chesterfield, Roanoke, Central Shenandoah. 
     * For health districts that span multiple counties, pick the county with the highest population for the mask survey and name the county that you're considering.

Pay attention to detail and the visualization principles we have discussed in class when designing your charts.  Each of your charts should have the same look and feel (color palette, fonts, etc.). In your report (see below), you will describe the design decisions you have made, so take notes along the way as you work through your design process. 

### Part 1 - Using Application
Choose an application (Excel, Google Sheets, or Tableau) to create the charts.

### Part 2 - Using Programming Language/API
Choose either R or Vega-Lite and re-create the charts you made in Part 1.  Strive to have both sets of charts look as similar as possible.

### Extra Credit
Create each of the charts in an application (Excel, Google Sheets, or Tableau), R, *and* Vega-Lite.

## Files to Include 

You must include all of these files in your GitHub repo (as applicable):

* edited data file(s) - *you may edit the original datafiles as needed*
* exported chart image (not screenshot) for each chart generated
* Excel: spreadsheet
* R: R code to generate the chart (can be in a RMarkdown notebook) 

In addition, for online formats include links to the source in your report:

* R: if you used Google Colab for your R chart, include the link to your notebook (save a copy to your GitHub repo)
* Vega-Lite: link to Observable notebook that generates the chart
* Google Sheets: link to shared Google Sheets (share with mweigle@<nolink>odu.edu)
* Tableau: publish your Tableau notebook to our class Tableau online site and include the link to your workbook in your report
  * see https://help.tableau.com/current/pro/desktop/en-us/publish_workbooks_share.htm
  * *set permissions so that only you and I can view the workbook*, see https://help.tableau.com/current/pro/desktop/en-us/publish_workbooks_permissions_add.htm

## Report
For this project, you can either directly write in Markdown in `report.md` or your can use R Markdown in `report.Rmd` and the Knit process to generate your `report.md`. (In any case, `report.md` is the file that I will use for grading.)

Your report should be a narrative, not just a set of bullet points. Treat this as a stand-alone document, not something that needs the assignment to be understood.  *Describe any insights you gained by exploring this data.  Did it prompt you to ask further questions?*

Directly include your charts as images (or generated R charts) in your report. If you have included the image files in your repo, also link to them so that they can be viewed at a larger size than in your report. At this stage, your charts do not need any interactive elements, so static images are acceptable.  

Other items to include:
* description of data used (specify attributes and their data types)
* for each chart (*only needs to be provided once for each type of chart, not for each implementation of the same chart*)
  * describe the marks and channels used and what attributes are mapped to which channels, justifying why these are appropriate choices
  * justify the choice of the chart idiom based on the data
  * describe the design decisions you made in creating the chart
  * describe how the chart you created answers one of the initial questions 
* describe any elements that you could not replicate between the application (Excel, Google Sheets, Tableau) versus programming language/API (R, Vega-Lite) charts
* compare your experience of using an application versus a programming language/API to implement the charts
* list of references - links to any examples that you used in completing this assignment (*use your own preference as to if the link should display the title or the URI, it may differ based on the particular URI*)

**Important:** Your report is the most important part of this assignment. I have not provided a template, but I expect your report to include your name, CS625-HW3, due date, and appropriate headings and Markdown markup for clarity and neatness. In addition, you will lose points if there are many spelling or grammatical errors. 

## Submission
Make sure that you have committed and pushed your local repo to GitHub.  Include "Ready to grade @weiglemc" in your final commit message. 

Submit the URL of your report (*not the URL of your repo*) in Blackboard:
* Click on HW3 under Assignments in Blackboard
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your `report.md` file into the edit box (should be something like https<nolink>://github.com/cs625-datavis-fall20/hw3-arrange-*username*/blob/master/report.md)
* Make sure to "Submit" your assignment.
