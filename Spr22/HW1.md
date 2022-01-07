*This is the public posting of the assignment. See Blackboard for the invite link to make your submission in your own repository in the class organization*

# Homework 1: Tool Setup

**Due:** January 20, 20222 by 11:59pm

The goal of this week's assignment is to get you set up for the rest of the semester.  You'll explore Git and GitHub, R and RStudio, Markdown, Google Colab, Tableau, and Observable with Vega-Lite.

*For this assignment only -- you may ask others in the class for help with these setup tasks.  Please use our Blackboard Discussion Board for these questions so that others may benefit from the answers.*

## Reports

Each HW assignment this semester will require you to write an accompanying report. These reports must be written in Markdown (or RMarkdown and knit to Markdown, see below).

### Formatting Reports

I've provided a template file ([`report.Rmd`](report.Rmd)) that can be edited for this assignment. All reports must include your name, HW number, class, and due date. In the template, use the "title" header for the HW number, "author" header for your name (*make sure to replace my name with yours*), and "date" header for the HW due date. 

The questions appear in *italics*, and your answers should be in non-italic text.

You may use existing code, but you must document and reference where you adapted the code -- give credit where credit is due! *Use without attribution is plagiarism!* All reports must have a section labeled "References" for listing the outside resources you consulted.

Before submitting your report, Knit your report to Markdown (should produce `report.md`), commit and push the files to your remote GitHub repo, and then view `report.md` on GitHub to make sure that the formatting is done properly and all needed files have been included. (Instructions on how to do this are given as part of the exercises below.)

### Submitting Reports

We will be using [GitHub Classroom](https://classroom.github.com/) for submitting HW assignments. Each HW assignment will have an invitation link available in Blackboard. When you accept the assignment, a new GitHub repository (repo) will be created for you.

Usually the new repo will only contain a README.md file with the assignment instructions. For some assignments, the repo may also contain data files needed to complete the assignment.

Before you submit your assignment, make sure that your GitHub repo contains all scripts, code, output files, and images needed to complete the assignment and your report.

## Git, GitHub

Git is a version control system for tracking changes in source code, used in the popular [GitHub](https://github.com) code hosting platform.  To become familiar with the basics of Git, read [git - the simple guide](https://rogerdudler.github.io/git-guide/).

If you do not have one already, you must create a GitHub account. I recommend a username that incorporates at least part of your actual name (e.g., mine is [Faryaneh](https://github.com/Faryaneh)). If you already have a GitHub account, you do not need to create a new one for this class.

Follow the instructions at [github-classroom-for-students](https://github.com/odu-cs625-datavis/github-classroom-for-students/blob/master/README.md) through the section "Make a local change, commit, and push and confirm the local change propogated to the GitHub Remote" to get setup with GitHub. You'll work through the remaining steps later.

[Mr. Thomas Kennedy](https://www.cs.odu.edu/~tkennedy/) has a nice introduction and walkthrough of Git available.  Read through [his materials](https://git.cs.odu.edu/tkennedy/git-workshop/-/wikis/Git-Workshop) and work through all of the exercises in the "Setting Up a Local Git Repository" section to create a repository, make changes, commit them locally, and then create a remote repo at GitHub. Once you have created the remote repo on GitHub, make the repo public or add me as a collaborator (Faryaneh).

* In the "Adding a Remote" section, note that 1) you will be using GitHub, not GitLab, and 2) Mr. Kennedy's example output is based on using GitLab and git-community<nolink>.cs.odu.edu, so your output will be slightly different.

Now, answer the following questions in `report.Rmd`:

1. What is your GitHub username?
1. What is the URL of your remote GitHub repo (created through Mr. Kennedy's exercises)?

## R, RStudio

[R](https://www.r-project.org) is a language and environment for statistical computing and graphics, and [RStudio](https://www.rstudio.com) is a widely-used open-source IDE for R.

Follow the instructions at [github-classroom-for-students](https://github.com/odu-cs625-datavis/github-classroom-for-students/blob/master/README.md) to get setup with GitHub and RStudio (start where you left off from before, at the "Steps for downloading and editing assignments from GitHub Classroom" section). If you are not familiar with the command-line, I would encourage you to use RStudio to ensure that your assignment updates are pushed back to GitHub.

We will be using some of the [R for Data Science](https://r4ds.had.co.nz) tutorials to setup and get a quick introduction to R. To finish the your R setup, read and follow the instructions from [Section 1.4.3 (The tidyverse)](https://r4ds.had.co.nz/introduction.html#the-tidyverse) through [Section 1.6 (Getting help and learning more)](https://r4ds.had.co.nz/introduction.html#getting-help-and-learning-more).

## Markdown, R Markdown

Markdown is a lightweight markup language that is often used in GitHub. Your reports will be written in R Markdown, which is a special flavor of Markdown that can include R code snippets.  

Here are some helpful links for Markdown and R Markdown:

* [Markdown Basic Syntax](https://www.markdownguide.org/basic-syntax)
* [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* [Mastering Markdown](https://guides.github.com/features/mastering-markdown/) (GitHub flavor)
* [R Markdown Introduction](https://rmarkdown.rstudio.com/lesson-1.html)
* [Add Images to an R Markdown Report](https://www.earthdatascience.org/courses/earth-analytics/document-your-science/add-images-to-rmarkdown-report/)

For this next section, read and work from [Section 27 (R Markdown)](https://r4ds.had.co.nz/r-markdown.html) through [Section 27.4 (Code chunks)](https://r4ds.had.co.nz/r-markdown.html#code-chunks) (you can skip Section 27.4.4 on Caching).  Working the Exercises in the tutorial is encouraged, but not required. 

Enter your answers to the following exercises in `report.Rmd`:

1. Create a bulleted list with at least 3 items
1. Write a single paragraph that demonstrates the use of *italics*, **bold**, ***bold italics***, `code`, and includes a link. The paragraph does not have to make sense.
1. Create a level 3 heading

## R

For a quick introduction to R, we'll continue working through some of the [R for Data Science](https://r4ds.had.co.nz) tutorials.  Start with [Section 3 (Data Visualization)](https://r4ds.had.co.nz/data-visualisation.html) and read through [Section 3.2 (First steps)](https://r4ds.had.co.nz/data-visualisation.html#first-steps) and then skip to [Section 3.4 (Common Problems)](https://r4ds.had.co.nz/data-visualisation.html#common-problems).

Complete questions 2-4 of the [Exercises in Section 3.2.4](https://r4ds.had.co.nz/data-visualisation.html#exercises) and enter your answers in `report.Rmd`.  For Question 4, in addition to explaining the answer to the question, include runnable R code (i.e., code chunk) in your report. 

We'll come back to some of the more advanced data visualizations later.  For now, skip to [Section 4 (Workflow: basics)](https://r4ds.had.co.nz/workflow-basics.html) and work through the entire section.

Complete question 2 of the [Practice exercises in Section 4.4](https://r4ds.had.co.nz/workflow-basics.html#practice) and enter your answer in `report.Rmd`. State what the problems were as well as including runnable R code that works in your report.

## Google Colab

[Google Colab](https://colab.research.google.com/) is a project to host Python-based Jupyter notebooks in the cloud. It also supports R notebooks, so we'll look at many of our R examples using this service. For more information about Google Colab, see their [FAQ](https://research.google.com/colaboratory/faq.html).

Make sure you're logged into a Google account (either a personal one or your ODU student account).

Open [Overview of Colaboratory Features](https://colab.research.google.com/notebooks/basic_features_overview.ipynb). Walk through and execute the examples shown. Experiment with changing some of the code and re-execute the cells.  Below each cell you edit, create a new Text cell that indicates you made an edit.  You can describe what you changed or even just write "EDIT MADE HERE".

File > Save a copy in Drive. In the Google Drive document that opens, click on Share, then click "Change to anyone with the link", then click "Copy link" and include that link in your `report.Rmd`.

Create a new [Google Colab R notebook](https://colab.research.google.com/#create=true&language=r).

Add a cell for each of the corrected commands from question 2 of the [Practice exercises in Section 4.4](https://r4ds.had.co.nz/workflow-basics.html#practice).  *Don't forget to include `library(tidyverse)` in the first cell.*

File > Save a copy in Drive. In the Google Drive document that opens, click on Share, then click "Change to anyone with the link", then click "Copy link" and include that link in your `report.Rmd`.

## Tableau

Sign up for [Tableau for Students](https://www.tableau.com/academic/students) to get a free one-year Tableau license. 

There are several video tutorials available at <https://www.tableau.com/learn/tutorials/on-demand/getting-started>. You are encouraged, but not required, to watch at least the Getting Started one (25 minutes).

For this assignment, we'll cover part of the [Get Started with Tableau Desktop](https://help.tableau.com/current/guides/get-started-tutorial/en-us/get-started-tutorial-home.htm) tutorial.  Work through [Step 3: Focus your results](https://help.tableau.com/current/guides/get-started-tutorial/en-us/get-started-tutorial-focus.htm).  

After you have created the final bar chart displaying the data from the South region, pick one of the other regions to display and save the chart as an image (*don't just take a screenshot*).  Save the image file in your repo (*no spaces in the filename*) and include the image in your `report.Rmd` (see [Add Images to an R Markdown Report](https://www.earthdatascience.org/courses/earth-analytics/document-your-science/add-images-to-rmarkdown-report/)).  Describe any conclusions you can draw from the chart.  

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

`markCircle()`

1. Pass an option of `{ size: 200 }` to `markCircle()`.
1. Try `markSquare` instead of `markCircle`.
1. Try `markPoint({ shape: 'diamond' })`.

`vl.x().fieldQ("Horsepower")`, ...

1. Change `Horsepower` to `Acceleration`
1. Swap what fields are displayed on the x- and y-axis

`vl.tooltip().fieldN("Name")`

1. Change `Name` to `Origin`.

Another example, `count()`

1. Remove the `vl.y().fieldN("Origin")` line.
1. Replace `count()` with `average("Miles_per_Gallon")`.

## References

Include links to any examples that you used in completing this assignment, including the tutorial examples that were given here. This will help you get into the habit of including such references.

## Submission

Make sure that you Knit your R Markdown so that a report.md file is created.  Also make sure that you have committed and pushed your local repo to GitHub.  Your repo should include at least `README.md` (this file), `report.Rmd`, `report.md` (the result of Knitting your R Markdown), and any image files you've included in your report.  Include "Ready to grade @Faryaneh" in your final commit message.

Submit the URL of your GitHub repo in Blackboard:

* Click on HW1 under Week 1 in Blackboard.
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your repo into the edit box
  * should be something like https<nolink>://github.com/odu-cs625-datavis/spring22-hw1-*username*
* Make sure to "Submit" your assignment.
