# Homework 5: Create Distribution Charts

*This is the public posting of the assignment. See Piazza for the invite link to make your submission in your own repository in the class organization.*

**Due:** October 29, 2019 *before* 9:30am  

The goal of this assignment is to practice creating distribution charts (histogram, eCDF, boxplot) in either R or Vega-Lite.

## Assignment

The following datasets contain varying types of distributions:

1) [movielens.csv](movielens.csv) - use the 'year' attribute - *represents the year that the movie was made*
2) [stars.csv](stars.csv) - use the 'magnitude' attribute - *represents the absolute magnitude of the star (function of the star's luminosity and distance to the star)*
3) [outlier_example.csv](outlier_example.csv)

Create a boxplot, eCDF, and two histograms (with different bin sizes) for each distribution using either R or Vega-Lite.  You may use either the standard R functions or [ggplot2](https://ggplot2.tidyverse.org) functions (used with the tidyverse package from our tutorials).

For R, these datasets are included in the ['dslabs' package](https://www.rdocumentation.org/packages/dslabs/versions/0.7.1).  You can run `install.packages("dslabs")` the first time you want use it and then `library(dslabs)` to gain access to the datasets.

For Vega-Lite, I have exported CSV files and they are linked above.

**Extra Credit:** Complete the exercise with both R and Vega-Lite.

There are a set of resources for [plotting distributions in R](https://www.cs.odu.edu/~mweigle/CS625-F19/Links#toc3) and [plotting distributions in Vega-Lite](https://www.cs.odu.edu/~mweigle/CS625-F19/Links#toc7) on the [class Links page](https://www.cs.odu.edu/~mweigle/CS625-F19/Links).  I *strongly encourage* you to read the documentation for these functions before you search the web for examples.

## Report

Your report is an important part of this assignment. I expect your report to include your name, CS625-HW5, date, and appropriate headings and Markdown markup for clarity and neatness. You will lose points if there are many spelling or grammatical errors. 

In your report, you must describe each of your charts and discuss the advantages and disadvantages of each type of chart idiom for each of the distributions. Which idiom provides the clearest picture of each distribution?

For R charts, use RMarkdown and produce runnable R code in your report.  

For Vega-Lite charts, include the chart image and provide a link to your Observable notebook.

As always, you must include a section titled "References", including links to any examples that you used in completing this assignment.

## Submission
Submit the URL of your report in Blackboard:
* Click on HW5 under Homeworks
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your `report.md` file into the edit box (should be something like https<nolink>://github.com/cs625-datavis-fall19/hw5-distributions-*username*/blob/master/report.md)
* Make sure to "Submit" your assignment.
