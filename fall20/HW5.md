*This is the public posting of the assignment. See Blackboard for the invite link to make your submission in your own repository in the class organization*

# Homework 5: Create Distribution Charts

**Due:** Thursday, October 29, 2020 by 11:59pm

The goal of this assignment is to practice creating distribution charts (histogram, eCDF, boxplot) in either R or Vega-Lite.

## Assignment

Create a boxplot, eCDF, and two histograms (with different bin sizes) for the distributions below using either R or Vega-Lite.  You may use either the standard R functions or [ggplot2](https://ggplot2.tidyverse.org) functions (used with the tidyverse package from our tutorials).

The following datasets contain varying types of distributions:

1) [NYT Mask Usage Survey dataset](https://github.com/nytimes/covid-19-data/tree/master/mask-use)
   * for the boxplot, show the distributions for all of the answers (Never, Rarely, Sometimes, Frequently, Always) on the same chart (each answer will have a separate boxplot glyph)
   * for eCDF and histograms, show the distribution of the levels of Frequently/Always mask usage (combine these columns)

2) [US Census Bureau County Population dataset](https://www.census.gov/data/datasets/time-series/demo/popest/2010s-counties-total.html#par_textimage_70769902)
   * for all charts, show the distribution of the population of all counties in the US as of the 2010 Census (CENSUS2010POP column)
   * your boxplot chart will just have a single boxplot glyph
   
3) [US Census Bureau State Population dataset](https://www.census.gov/data/tables/time-series/demo/popest/2010s-state-total.html#par_textimage)
   * for the boxplot, show the distributions for the 2019 birth rates (RBIRTH2019 column), death rates (RDEATH2019 column), and migration rates (RNETMIG2019 column) for all the states in the US (will result in 3 separate boxplot glyphs)
   * for the eCDF and histograms, pick one of the above (birth rates, death rates, or migration rates)

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

Note that you will be creating a total of 12 charts (4 charts for each of the 3 distributions).

Make sure to include informative axis labels and chart titles.

**Extra Credit:** Complete the exercise with both R and Vega-Lite.

## Report

Your report is an important part of this assignment. I expect your report to include your name, CS625-HW5, date, and appropriate headings and Markdown markup for clarity and neatness. You will lose points if there are many spelling or grammatical errors. 

In your report, you must include the following items:
* describe each of your charts
* what conclusions or observations can you draw from the charts?
* discuss the advantages and disadvantages of each type of chart idiom for each of the distributions
* what effect did changing the bin size of the histogram have on the conclusions you were able to draw from the chart?
* which idiom provides the clearest picture of each distribution?

For R charts, use RMarkdown and produce runnable R code in your report.  

For Vega-Lite charts, include the chart image and provide a link to your Observable notebook.

As always, you must include a section titled "References", including links to any examples that you used in completing this assignment.


## Useful Links

Here are a set of references that you might find useful (you do not have to cite these in your report).

Resources for plotting distributions in R:
* Boxplot - https://www.rdocumentation.org/packages/graphics/versions/3.6.1/topics/boxplot, https://www.datamentor.io/r-programming/box-plot/
* Histogram - https://www.rdocumentation.org/packages/graphics/versions/3.6.1/topics/hist, https://www.datamentor.io/r-programming/histogram/
* eCDF - https://www.rdocumentation.org/packages/stats/versions/3.6.1/topics/ecdf, https://r-dir.com/blog/2014/03/cdfs-in-r.html

Resources for plotting distributions in R with ggplot2:
* Boxplot - https://ggplot2.tidyverse.org/reference/geom_boxplot.html
* Histogram - https://ggplot2.tidyverse.org/reference/geom_histogram.html
* eCDF - https://ggplot2.tidyverse.org/reference/stat_ecdf.html

Resources for plotting distributions in Vega-Lite:
* Boxplot - https://vega.github.io/vega-lite/docs/boxplot.html
* Histogram - https://vega.github.io/vega-lite/docs/bin.html, https://vega.github.io/vega-lite/docs/bin.html#histogram
* eCDF - https://vega.github.io/vega-lite/docs/window.html, https://vega.github.io/vega-lite/docs/window.html#cumulative-frequency-distribution

I *strongly encourage* you to read the documentation for these functions before you search the web for examples.

## Submission
Make sure that you have committed and pushed your local repo to GitHub.  Include "Ready to grade @weiglemc" in your final commit message. 

Submit the URL of your report in Blackboard:
* Click on HW5 under Assignments in Blackboard
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your `report.md` file into the edit box (should be something like https<nolink>://github.com/cs625-datavis-fall20/hw5-distributions-*username*/blob/master/report.md)
* Make sure to "Submit" your assignment.
