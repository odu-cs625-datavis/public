# Homework 1: Tool Setup

*This is the public posting of the assignment. See Piazza for the invite link to make your submission in your own repository in the class organization.*

**Due:** September 3, 2019 *before* 9:30am

The goal of this week's assignment is to get you set up for the rest of the semester.  You'll explore Git (and GitHub), R (and RStudio), Tableau, and Observable with Vega-Lite.

*For this assignment only -- you may ask others in the class for help with these setup tasks.*

You will write a report to be compiled while completing these tasks.  Instructions on how to do this will be provided as part of the following sections.

## Setting Up Git, GitHub, R, RStudio

Git is a version control system for tracking changes in source code, used in the popular [GitHub](https://github.com) code hosting platform.  To become familiar with the basics of Git, read [git - the simple guide](https://rogerdudler.github.io/git-guide/).

[R](https://www.r-project.org) is a language and environment for statistical computing and graphics, and [RStudio](https://www.rstudio.com) is a widely-used open-source IDE for R.

Follow the instructions at [github-classroom-for-students](https://github.com/cs625-datavis-master/github-classroom-for-students/blob/master/README.md) to get setup with GitHub and RStudio. If you are not familiar with the command-line, I would encourage you to use RStudio to ensure that your assignment updates are pushed back to GitHub. 

We will be using some of the [R for Data Science](https://r4ds.had.co.nz) tutorials to setup and get a quick introduction to R. To finish the your R setup, read and follow the instructions from [Section 1.4.3 (The tidyverse)](https://r4ds.had.co.nz/introduction.html#the-tidyverse) through [Section 1.6 (Getting help and learning more)](https://r4ds.had.co.nz/introduction.html#getting-help-and-learning-more). 

Reports, required for almost all assignments, will be done using R Markdown (see below). The template file [`report.Rmd`](report.Rmd) has been provided for you to edit in your own repository. The questions are provided in *italics*. Your answers should be in non-italic text.

## R Markdown

Your reports (such as `report.Rmd`) will be written in R Markdown, which is a special flavor of Markdown that can include R code snippets.  There are several Markdown and R Markdown resources and guides in the [Markdown section](https://www.cs.odu.edu/~mweigle/CS625-F19/Links#markdown) of the class Links page.

For this next section, read and work from [Section 27 (R Markdown)](https://r4ds.had.co.nz/r-markdown.html) through [Section 27.3 (Text formatting with Markdown)](https://r4ds.had.co.nz/r-markdown.html#text-formatting-with-markdown).  Working the Exercises in the tutorial is encouraged, but not required.  We will come back to including R code in R Markdown reports later.

Enter your answers to the following required exercises in `report.Rmd`:

1. Create an ordered bulleted list with at least 3 items
1. Write a paragraph that demonstrates the use of *italics*, **bold**, ***bold italics***, and `inline code`.
1. Create an example of a fenced code block.
1. Create a level 4 heading

## R

For a quick introduction to R, we'll continue working through some of the [R for Data Science](https://r4ds.had.co.nz) tutorials.  Start with [Section 3 (Data Visualization)](https://r4ds.had.co.nz/data-visualisation.html) and read through [Section 3.2 (First steps)](https://r4ds.had.co.nz/data-visualisation.html#first-steps) and then skip to [Section 3.4 (Common Problems)](https://r4ds.had.co.nz/data-visualisation.html#common-problems). 

Complete the [Exercises in Section 3.2.4](https://r4ds.had.co.nz/data-visualisation.html#exercises) and enter your answers in `report.Rmd`.  For Questions 1, 4, and 5, in addition to explaining the answer to the question, include runnable R code in your report. (See [Section 27.4](https://r4ds.had.co.nz/r-markdown.html#code-chunks) for how to include runnable R code.)

We'll come back to some of the more advanced data visualizations later.  For now, skip to [Section 4 (Workflow: basics)](https://r4ds.had.co.nz/workflow-basics.html) and work through the entire section. 

Complete the [Practice exercises in Section 4.4](https://r4ds.had.co.nz/workflow-basics.html#practice) and enter your answers in `report.Rmd`. For Questions 1 and 2, in addition to explaining the answer to the question, include runnable R code in your report.

## Tableau

Sign up for [Tableau for Students](https://www.tableau.com/academic/students) to get a free one-year Tableau license.  I will also have license keys available.

There are several video tutorials available at https://www.tableau.com/learn/tutorials/on-demand/getting-started. You are encouraged, but not required, to watch at least the Getting Started one (25 minutes).

For this assignment, we'll cover part of the [Get Started with Tableau Desktop](https://help.tableau.com/current/guides/get-started-tutorial/en-us/get-started-tutorial-home.htm) tutorial.  Work through [Step 3: Focus your results](https://help.tableau.com/current/guides/get-started-tutorial/en-us/get-started-tutorial-focus.htm).  

After you have created the final bar chart displaying the data from the South region, pick one of the other regions to display and save the chart as an image (*don't just take a screenshot*).  Save the image file in your repo (*no spaces in the filename*) and include the image in your `report.Rmd`.  You will also be asked to describe any conclusions you can draw from the chart.  See [Add Images to an R Markdown Report](https://www.earthdatascience.org/courses/earth-analytics/document-your-science/add-images-to-rmarkdown-report/) for help on inserting the image in your report.

## Observable and Vega-Lite

[Observable](https://observablehq.com) is a notebook platform that is based on JavaScript. It's similar to other notebooks, but [R Notebooks](https://bookdown.org/yihui/rmarkdown/notebook.html) are based on R and [Jupyter Notebooks](https://jupyter.org) were originally based on Python. Observable can be tied to your GitHub account, so to get started, make sure that you're logged into GitHub.

Open the [Observable 5 Minute Intro](https://observablehq.com/@observablehq/five-minute-introduction?collection=@observablehq/introduction) and fork the notebook (click the 'Fork' button at the top right).  

Read through the notebook and experiment by making changes in the cells, running the code, and seeing how the output changes. Make sure to note the changes you make so that you can report them in your `report.Rmd`. Create a new cell at the top with your name and CS 625, Fall 2019.  Then publish your notebook (click the 'Publish' button at the top right) and enter the URL of your notebook in `report.Rmd`. 

Add the answer to the following question to `report.Rmd`:

* What happens when you select a range of items in the scatterplot at the end of the notebook?

[Vega-Lite](http://vega.github.io/vega-lite/) is a high-level language for building interactive visualizations on the web. It is based on [D3](https://d3js.org).  Because it is JavaScript-based, Vega-Lite can be embedded in Observable notebooks.

Open the [Introduction to Vega-Lite](https://observablehq.com/@uwdata/introduction-to-vega-lite) notebook on Observable and fork the notebook.

Read through the notebook and experiment by making changes in the cells, running the code, and seeing how the output changes. Make sure to note the changes you make so that you can report them in your `report.Rmd`.  Create a new cell at the top with your name and CS 625, Fall 2019.  Then publish your notebook (click the 'Publish' button at the top right) and enter the URL of your notebook in `report.Rmd`. 

Save one of the images that you generate (make sure that it's one that you've modified from the original), save the file in your repo, and insert the image in `report.Rmd`. *Note: The right-click menu in Observable is different when using Safari and doesn't include 'Save Image As'. You might want to use Chrome or Firefox.*

## References
Include links to any examples that you used in completing this assignment, including the tutorial examples that were given here. This will help you get into the habit of including such references.

## Submission

Make sure that you have committed and pushed your local repo to GitHub.  Your repo should include at least `README.md` (this file), `report.Rmd`, `report.md` (the result of Knitting your R Markdown), and any image files you've included in your report.

Submit the URL of your GitHub project in Blackboard:

* Click on HW1 under Homeworks
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your repo into the edit box
  * should be something like https<nolink>://github.com/cs625-datavis-fall19/hw1-setup-*username*
* Make sure to "Submit" your assignment.
