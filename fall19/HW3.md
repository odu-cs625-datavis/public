# Homework 3: Arrange Tables

*This is the public posting of the assignment. See Piazza for the invite link to make your submission in your own repository in the class organization.*

**Due:** October 1, 2019 *before* 9:30am (two weeks -- *but don't wait until next week to start!*)

The goal of this assignment is to practice choosing and implementing approriate chart idioms based on given data and questions.

## Dataset
The dataset we will examine comes from [NEST (Norfolk Emergency Shelter Team)](https://www.norfolk.gov/index.aspx?NID=1228), which is a coalition of churches that provides overnight shelter during the winter for adults experiencing homelessness.

[nest-data.csv](nest-data.csv) contains the following fields:  
* Date - night that shelter was provided
* Church - church or pair of churches where shelter was provided, multiple churches are delimited by a "/" character
* Women - number of women who were provided shelter
* Men - number of men who were provided shelter
* Turned Away - number of persons who were not able to be provided shelter because capacity had been reached
* Total Guests - sum of Women and Men columns
* Total Demand - sum of Total Guests and Turned Away columns

[nest-weather.csv](nest-weather.csv) contains the following fields:
* Date - night that shelter was provided
* Temp Low - low temperature
* Precipitation - amount of rain (inches), T = "trace" (less than 0.01 inches)
* Snow - amount of snowfall (inches), T = "trace" (less than 0.01 inches)
* Snow Depth - amount of snow on the ground (inches)

## Assignment

### Part 1 - Using Application

Choose an application (Excel, Google Sheets, or Tableau) to explore the dataset and create a chart for each of the following questions:

1. What was the breakdown of women vs. men who were provided shelter each night?
1. In total, how many guests were provided shelter by each church (or pair of churches)?
1. Is total demand for shelter affected by weather?

Pay attention to detail and the visualization principles we have discussed in class when designing your charts.  Each of your charts should have the same look and feel. In your report (see below), you will describe the design decisions you have made, so take notes along the way as you work through your design process. 

### Part 2 - Using Programming Language/API
Re-create each chart from Part 1 in either R or Vega-Lite.  Strive to have both sets of charts look as similar as possible.

***Extra Credit:*** Create each of the 3 charts in Tableau, R, *and* Vega-Lite.

## Files to Include 

You must include all of these files in your GitHub repo (as applicable):

* edited data file(s) - *you may edit the original datafiles as needed*
* exported chart image (not screenshot) for each chart generated
* Excel: spreadsheet
* R: R code to generate the chart (can be in a RMarkdown notebook)

In addition, for online formats include links to the source in your report:

* Google Sheets: link to shared Google Sheets (share with mweigle@odu.edu)
* Tableau: link to shared Tableau notebook
* Vega-Lite: link to Observable notebook that generates the chart

## Report
For this project, you can either directly write in Markdown in `report.md` or your can use R Markdown in `report.Rmd` and the Knit process to generate your `report.md`. (In any case, `report.md` is the file that I will use for grading.)

Your report should be a narrative, not just a set of bullet points. Treat this as a stand-alone document, not something that needs the assignment to be understood.

You may directly include your charts as images (or generated R charts) in your report or you may link to images contained in your GitHub repo. At this stage, your charts do not need any interactive elements, so static images are acceptable.  

Other items to include:
* description of data (specify attributes and their data types)
* for each chart (*only needs to be provided once for each type of chart, not for each implementation of the same chart*)
  * describe the marks and channels used and what attributes are mapped to which channels, justifying why these are appropriate choices
  * justify the choice of the chart idiom based on the data
  * describe the design decisions you made in creating the chart
  * describe how the chart you created answers one of the initial questions 
* describe any elements that you could not replicate between the application (Excel, Google Sheets, Tableau) versus programming language/API (R, Vega-Lite) charts
* compare your experience of using an application versus a programming language/API to implement the charts
* list of references - links to any examples that you used in completing this assignment

**Important:** Your report is the most important part of this assignment. I have not provided a template, but I expect your report to include your name, CS625-HW3, date, and appropriate headings and Markdown markup for clarity and neatness. In addition, you will lose points if there are many spelling or grammatical errors. 

## Submission
Submit the URL of your report (*not the URL of your repo*) in Blackboard:
* Click on HW3 under Homeworks
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your `report.md` file into the edit box (should be something like https<nolink>://github.com/cs625-datavis-fall19/hw3-arrange-*username*/blob/master/report.md)
* Make sure to "Submit" your assignment.
