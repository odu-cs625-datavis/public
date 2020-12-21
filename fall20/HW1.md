*This is the public posting of the assignment. See Blackboard for the invite link to make your submission in your own repository in the class organization*

# Homework 1: Tool Setup

**Due:** September 8, 2020 by 11:59pm

The goal of this week's assignment is to get you set up for the rest of the semester.  You'll explore Git (and GitHub), R (and RStudio), Tableau, and Observable with Vega-Lite. 

*For this assignment only -- you may ask others in the class for help with these setup tasks.  Please use Piazza and post in the `hw1` folder for these questions so that others may benefit from the answers.*

Reports, required for almost all assignments, will be done using R Markdown (see below). The template file [`report.Rmd`](report.Rmd) has been provided for you to edit in your own repository. The questions are provided in *italics*. Your answers should be in non-italic text.

## Git, GitHub 

Git is a version control system for tracking changes in source code, used in the popular [GitHub](https://github.com) code hosting platform.  To become familiar with the basics of Git, read [git - the simple guide](https://rogerdudler.github.io/git-guide/).

Follow the instructions at [github-classroom-for-students](https://github.com/cs625-datavis-master/github-classroom-for-students/blob/master/README.md) through the section "Make a local change, commit, and push and confirm the local change propogated to the GitHub Remote" to get setup with GitHub. You'll work through the remaining steps later.

Mr. Thomas Kennedy has a nice introduction and walkthrough of Git available.  Read through [his materials](https://git-community.cs.odu.edu/tkennedy/git-workshop/-/wikis/Git-Workshop) and work through all of the exercises in the "Setting Up a Local Git Repository" section to create a repository, make changes, commit them locally, and then create a remote repo at GitHub. Once you have created the remote repo on GitHub, make the repo public or add me as a collaborator (weiglemc)

Now, answer the following questions in `report.Rmd`:
1. What is your GitHub username?
1. What is the URL of your remote GitHub repo (created through Mr. Kennedy's exercises)?

## R, RStudio

[R](https://www.r-project.org) is a language and environment for statistical computing and graphics, and [RStudio](https://www.rstudio.com) is a widely-used open-source IDE for R.

Follow the instructions at [github-classroom-for-students](https://github.com/cs625-datavis-master/github-classroom-for-students/blob/master/README.md) to get setup with GitHub and RStudio (start where you left off from before, at the "Steps for downloading and editing assignments from GitHub Classroom" section). If you are not familiar with the command-line, I would encourage you to use RStudio to ensure that your assignment updates are pushed back to GitHub. 

We will be using some of the [R for Data Science](https://r4ds.had.co.nz) tutorials to setup and get a quick introduction to R. To finish the your R setup, read and follow the instructions from [Section 1.4.3 (The tidyverse)](https://r4ds.had.co.nz/introduction.html#the-tidyverse) through [Section 1.6 (Getting help and learning more)](https://r4ds.had.co.nz/introduction.html#getting-help-and-learning-more). 

## R Markdown

Your reports (such as `report.Rmd`) will be written in R Markdown, which is a special flavor of Markdown that can include R code snippets.  

Here are some helpful links for Markdown and R Markdown:
* [Markdown Basic Syntax](https://www.markdownguide.org/basic-syntax)
* [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* [Markdown on GitHub](https://help.github.com/en/categories/writing-on-github) -- it can be slightly different than regular Markdown
  * [Mastering Markdown](https://guides.github.com/features/mastering-markdown/) (GitHub flavor)
* [R Markdown Introduction](https://rmarkdown.rstudio.com/lesson-1.html)
* [Add Images to an R Markdown Report](https://www.earthdatascience.org/courses/earth-analytics/document-your-science/add-images-to-rmarkdown-report/)

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

Complete questions 1 and 2 of the [Practice exercises in Section 4.4](https://r4ds.had.co.nz/workflow-basics.html#practice) and enter your answers in `report.Rmd`. In addition to explaining the answer to the question, include runnable R code in your report.

## Tableau

Sign up for [Tableau for Students](https://www.tableau.com/academic/students) to get a free one-year Tableau license.  I will also have license keys available.

There are several video tutorials available at https://www.tableau.com/learn/tutorials/on-demand/getting-started. You are encouraged, but not required, to watch at least the Getting Started one (25 minutes).

For this assignment, we'll cover part of the [Get Started with Tableau Desktop](https://help.tableau.com/current/guides/get-started-tutorial/en-us/get-started-tutorial-home.htm) tutorial.  Work through [Step 3: Focus your results](https://help.tableau.com/current/guides/get-started-tutorial/en-us/get-started-tutorial-focus.htm).  

After you have created the final bar chart displaying the data from the South region, pick one of the other regions to display and save the chart as an image (*don't just take a screenshot*).  Save the image file in your repo (*no spaces in the filename*) and include the image in your `report.Rmd`.  You will also be asked to describe any conclusions you can draw from the chart.  See [Add Images to an R Markdown Report](https://www.earthdatascience.org/courses/earth-analytics/document-your-science/add-images-to-rmarkdown-report/) for help on inserting the image in your report.

## Observable and Vega-Lite

[Observable](https://observablehq.com) is a notebook platform that is based on JavaScript. It's similar to other notebooks, but [R Notebooks](https://bookdown.org/yihui/rmarkdown/notebook.html) are based on R and [Jupyter Notebooks](https://jupyter.org) were originally based on Python.  [Vega-Lite](http://vega.github.io/vega-lite/) is a high-level language for building interactive visualizations on the web. It is based on [D3](https://d3js.org).  Because it is JavaScript-based, Vega-Lite can be embedded in Observable notebooks.

Observable can be tied to your GitHub account, so to get started, make sure that you're logged into GitHub.

Open the [A Taste of Observable](https://observablehq.com/@observablehq/a-taste-of-observable) notebook and work through the examples and questions that it asks.  Report your answers in `report.Rmd`.

1. In the "New York City weather forecast" section, try replacing `Forecast: detailedForecast` with `Forecast: shortForecast`. Then press the blue play button  or use Shift-Return to run your change. What happens?

1. Under the scatterplot of temperature vs. name, try replacing `markCircle()` with `markSquare()`. Then press the blue play button  or use Shift-Return to run your change. What happens? How about `markPoint()`?

1. Under "Pick a location, see the weather forecast", pick a location on the map.  Where was the point you picked near?  (Be a little patient with the updates.)

1. The last visualization on this page is a "fancy" weather chart embedded from another notebook.  Click on the 3 dots next to that chart and choose 'Download PNG'.  Insert the PNG into your report.

Read through the [Introduction to Data](https://observablehq.com/@observablehq/introduction-to-data) notebook. There are no exercises to work, but this will be useful material for you going forward.

Open the [Charting with Vega-Lite](https://observablehq.com/@observablehq/vega-lite) notebook and work the "Try it Yourself" exercises listed below.  Record what happens when you make the changes in your report.

1. Pass an option of `{ size: 200 }` to `markCircle()`.

1. Try `markSquare` instead of `markCircle`.

1. Try `markPoint({ shape: 'diamond' })`.

1. Change `Horsepower` to `Acceleration`

1. Swap what fields are displayed on the x- and y-axis

1. Change `Name` to `Origin`.

1. Remove the `vl.y().fieldN("Origin")` line.

1. Replace `count()` with `average("Miles_per_Gallon")`.

## References
Include links to any examples that you used in completing this assignment, including the tutorial examples that were given here. This will help you get into the habit of including such references.

## Submission

Make sure that you Knit your R Markdown so that a report.md file is created.  Also make sure that you have committed and pushed your local repo to GitHub.  Your repo should include at least `README.md` (this file), `report.Rmd`, `report.md` (the result of Knitting your R Markdown), and any image files you've included in your report.  Include "Ready to grade @weiglemc" in your final commit message. 


Submit the URL of your GitHub project in Blackboard:

* Click on HW1 under Week 1 in Blackboard. 
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your repo into the edit box
  * should be something like https<nolink>://github.com/cs625-datavis-fall20/hw1-setup-*username*
* Make sure to "Submit" your assignment.
