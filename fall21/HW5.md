*This is the public posting of the assignment. See Blackboard for the invite link to make your submission in your own repository in the class organization*

# Homework 5: Analyzing Data Using Distribution Charts

**Due:** Tuesday, November 9, 2021 by 11:59pm 

The goal of this assignment is gain experience creating distribution charts (histogram, eCDF, boxplot) and using them to help guide further analysis of the underlying data.

## Assignment

### Part 1: Create Distribution Charts

To start your analysis, create a boxplot, eCDF, and histogram for the distributions described below using R, Vega-Lite, or Python.

Pick one of the two datasets to work with:

1) [US Census Bureau County Population dataset](https://www.census.gov/data/datasets/time-series/demo/popest/2010s-counties-total.html#par_textimage_70769902) (CO-EST2019-alldata)
   * for the boxplot, show the distribution of the population of all counties in the US as of the 2010 Census (`CENSUS2010POP`), the 2015 estimate (`POPESTIMATE2015`), and the 2019 estimate (`POPESTIMATE2019`) (should result in 3 separate boxplot glyphs in a single chart)
   * for the eCDF and histogram, show the distribution of the population of all counties in the US as of the 2010 Census (`CENSUS2010POP` column)
   
2) [US Census Bureau State Population dataset](https://www.census.gov/data/tables/time-series/demo/popest/2010s-state-total.html#par_textimage) (NST-EST2019-alldata)
   * for the boxplot, show the distributions for the 2019 birth rates (`RBIRTH2019` column), death rates (`RDEATH2019` column), and migration rates (`RNETMIG2019` column) for all the states in the US (should result in 3 separate boxplot glyphs in a single chart)
   * for the eCDF and histogram, pick one of the above columns (birth rates, death rates, or migration rates)

Feel free to pull the datasets into a separate application and format it as needed.  Note that both R and Unix have powerful features for manipulating data that you might want to explore. As an example, here's a snippet of using the `awk` Unix shell command to extract only the relevant columns from the state dataset:
```
% awk -F ',' 'NR==1 || NR>6 {print $5, $106, $115, $151}' nst-est2019-alldata.csv | head -4
NAME RBIRTH2019 RDEATH2019 RNETMIG2019
Alabama 11.707442426 11.005972301 2.4837435218
Alaska 13.678474709 6.5712859757 -12.03122145
Arizona 11.351869511 8.3845793175 13.687161112
```
* `NR==1 || NR>6` prints the first row (header) and then skips the next 5 rows (US, and regions)
* `$` is used to select the column number

For this part, you must include the following items in your report:
* describe any data manipulation you needed to perform before creating the charts
* describe each of your charts and how they were created (explain the code you used and include code snippets)
* discuss the advantages and disadvantages of each type of chart idiom for showing these distributions (talk specifically about these distributions, not just their advantages and disadvantages generally)
* name 1-2 simple observations you can draw from each chart

### Part 2: Further Analysis

Use the charts that you created in Part 1 to guide further investigation of the data.  I expect to see additional charts created in this part.  This may be additional histograms with a different bin size (to investigate smaller details or to see the larger picture) or other types of charts that reveal something interesting. 

State at least 2 interesting findings about the data and explain how you used one or more of the distribution charts to guide the investigation into this finding. These findings must be something more than a simple observation from the base charts. For example, I want something more than "80% of the counties in the US have less than 1 million people" (this may or may not be true, it's just an example).

It is fine if you want to consult additional datasets as part of your analysis.

I expect to see a full explanation of your analysis in your report.  How did you arrive at your findings by starting with one of the distribution charts?

### Things to Remember
* Look at the data before you start creating charts.
* Do a sanity-check on your results.  Do they make sense? 
* Review the in-class tutorial and read the documentation before you search the web for examples.
* Include informative axis labels and chart titles.
* When inserting images into your report, make sure that the entire chart can be viewed without scrolling.

## Report

Your report is an important part of this assignment. I expect your report to include your name, CS625-HW5, date, and appropriate headings and Markdown markup for clarity and neatness. You will lose points if there are many spelling or grammatical errors. 

What to include for different tools:
* R - either use RMarkdown and produce runnable R code in your report, or include the chart images in your report and your R script in the repo
* Vega-Lite - include the chart images in your report and provide a link to your Observable notebook
* Python - include the chart images in your report and your Python script in the repo

As always, you must include a section titled "References", including links to any examples that you used in completing this assignment.

## Submission
Make sure that you have committed and pushed your local repo to GitHub.  Include "Ready to grade @weiglemc @javedulferdous" in your final commit message. 

Submit the URL of your report in Blackboard:
* Click on HW5 under Assignments in Blackboard
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your `report.md` file into the edit box (should be something like https<nolink>://github.com/odu-cs625-datavis/fall21-hw5-*username*/blob/master/report.md)
* Make sure to "Submit" your assignment.
