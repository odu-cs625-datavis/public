# Homework 4: Arrange Tables 

**Due:** Thursday, October 20, 2022 by 11:59pm 

The goal of this assignment is to propose and implement charts based on questions asked about real-world data.  *Read through the entire assignment before starting.*

## Datasets
We are going to use two datasets from the [Virginia Department of Health's COVID-19 Resources](https://www.vdh.virginia.gov/coronavirus/covid-19-in-virginia/).  The datasets are made available through the [Virginia Open Data Portal](https://data.virginia.gov).

1. Weekly cases by vaccination status by health region  
https://data.virginia.gov/dataset/VDH-COVID-19-PublicUseDataset-Cases-by-Vaccination/vsrk-d6hx
> This dataset includes the number of COVID-19 infections, hospitalizations, and deaths for each health region in Virginia by the week of onset/specimen collection and by vaccination status.

2. Daily vaccines administered by health district  
https://data.virginia.gov/dataset/VDH-COVID-19-PublicUseDataset-Vaccines-DosesAdmini/28k2-x2rj
> This dataset includes the number of COVID-19 vaccine doses administered for each locality in Virginia by administration date and by facility type. The data set increases in size daily and as a result, the dataset may take longer to update; however, it is expected to be available by 12:00 noon daily.

For each dataset, you can click the Export button on the dataset page to download the CSV, or you can use the API endpoint to access the data ([example Observable notebook](https://observablehq.com/d/2b7bf74dbcb9dacf), [example R Google Colab notebook](https://github.com/odu-cs625-datavis/public/blob/main/Spr22/R_SODA_API_for_VDH_data.ipynb), [example Python/Pandas Google Colab notebook](https://github.com/odu-cs625-datavis/public/blob/main/Spr22/Va_Open_Data_Portal_API_Example.ipynb)). 

Since one dataset is aggregated on health regions and the other is aggregated on localities (but includes health districts), you may need this information about [Virginia health regions, districts, and localities](https://www.vdh.virginia.gov/content/uploads/sites/182/2020/08/VA-regions_districts_localities.pdf) (pdf)

## Assignment

As you work through this, pay attention to detail and the visualization principles we have discussed in class when designing your charts.  Charts must have appropriately labeled axes and appropriate unit formats. In your report ([see below](#report)), you will describe the design decisions you have made, so take notes along the way as you work through your design process. 

You may use whatever tool(s) you wish to manipulate the data and create the charts.

### Part 1

Use dataset 1 to create a chart to answer the question, "How has the weekly rate of COVID-19 cases in Virginia changed over time based on vaccination status?". (Though I'll use cases here, you may show cases, hospitalizations, or deaths.)

#### Calculating the Weekly Rate

Since there are different numbers of people in various vaccination states over time, we want to normalize the values instead of just presenting the raw numbers.  For instance, if there are 10 people in each category that contract COVID, but there are 100 times more people who are fully vaccinated than unvaccinated, that makes a big difference in the case rate.

Typically these numbers are presented as rates per 100,000 people.  Dataset 1 contains an attribute that can help us calculate this rate.  The `population_denominator` attribute provides an estimate of the number of people in the state with a certain vaccination status for that week.  

The general formula is `rate_per_100k = (cases / population_denominator) * 100000`. For example, if there were 100 COVID cases among unvaccinated in the state in one week and there were 2,000,000 people unvaccinated (represented in `population_denominator`), then  

`rate_per_100k = (100 / 2,000,000) * 100000 = 5`  

This means that this rate is equivalent to 5 cases in a population of 100,000.


### Part 2

Use dataset 2 to create a chart to answer the question, "For each health district in Virginia, what proportion of all 1st doses were of the Pfizer vaccine?". 

Remove or ignore the "health districts" labeled "Out of State" and "Not Reported".

### Part 3

Propose two questions that require data from dataset 1 and dataset 2 to be combined to answer.  Describe what data manipulation would need to be done to answer each question.  *Sketch* a chart that could be used the answer each question.  Justify your visualization idiom choice.


## Files to Include 

You must include all of these files in your GitHub repo (as applicable):

* edited data file(s) - *you may edit the original datafiles as needed*
* exported chart image (not screenshot) for each chart generated
* Excel: spreadsheet
* R: R code to generate the chart (can be in a RMarkdown notebook) 

In addition, for online formats include links to the source in your report:

* R or Python: if you used Google Colab, include the link to your notebook (save a copy to your GitHub repo)
* Vega-Lite: link to Observable notebook that generates the chart
* Google Sheets: link to shared Google Sheets (share with poursardar@<nolink>cs.odu.edu and kgarg001@<nolink>odu.edu)
* Tableau: publish your Tableau notebook to our class Tableau online site and include the link to your workbook in your report
  * see https://help.tableau.com/current/pro/desktop/en-us/publish_workbooks_share.htm
  * *set permissions so that only you and I can view the workbook*, see https://help.tableau.com/current/pro/desktop/en-us/publish_workbooks_permissions_add.htm

## Report
For this project, you can either directly write in Markdown in `report.md` or your can use R Markdown in `report.Rmd` and the Knit process to generate your `report.md`. (In any case, `report.md` is the file that I will use for grading.)

Your report should be a narrative, not just a set of bullet points. Treat this as a stand-alone document, not something that needs the assignment to be understood.  *Describe any insights you gained by exploring this data.  Did it prompt you to ask further questions?*

Directly include your charts as images (or generated R charts) in your report.  At this stage, your charts do not need any interactive elements, so static images are acceptable.  

Other items to include:
* description of data used (specify attributes and their data types)
* for each chart
  * explain any data manipulation you performed
  * describe the marks and channels used and what attributes are mapped to which channels, justifying why these are appropriate choices
  * justify the choice of the chart idiom based on the data
  * describe the design decisions you made in creating the chart
  * describe how the chart you created answers the question that was asked
* list of references - links to any examples that you used in completing this assignment

**Important:** Your report is an important part of this assignment. I have not provided a template, but I expect your report to include your name, CS625-HW4, due date, and appropriate headings and Markdown markup for clarity and neatness. You will lose points if there are many spelling or formatting errors. 

## Submission
Make sure that you have committed and pushed your local repo to GitHub.  Include "Ready to grade @Faryaneh @Kritikagarg" in your final commit message. 

Submit the URL of your report (*not the URL of your repo*) in Canvas:
* Click on HW4 under Assignments in Canvas
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your `report.md` file into the edit box (should be something like https<nolink>://github.com/odu-cs625-datavis/fall22-hw4-*username*/blob/master/report.md)
* Make sure to "Submit" your assignment.
