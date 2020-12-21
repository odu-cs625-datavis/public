# Homework 7: Generating Questions from Real-World Data

*This is the public posting of the assignment. See Piazza for the invite link to make your submission in your own repository in the class organization.*

**Due:** November 19, 2019 *before* 9:30am (2 weeks)

The goal of this assignment is to use EDA techniques to generate questions from a dataset(s) and propose charts to address those questions. 

## Assignment

Use the EDA process to explore a dataset of your choice.  Through this process, you should generate at least 2 detailed questions that can be most effectively answered through visualization (rather than just directly reporting the results).  Sketch (on paper) or draft (using the tool of your choice) charts that could address and answer those questions.

The [Data Sources page](https://www.cs.odu.edu/~mweigle/CS625-F19/Data) contains links to several public data sources (including the `dslabs` R package that we've previously explored). Be careful about the size of the dataset. You probably want on the order of 100s-1000s of items rather than millions.

Note that you might need to combine multiple datasets to answer the questions you develop.  For example, combining the NEST guest counts with weather data to investigate how weather may affect demand for shelter.

**Important:** No two students may choose the same dataset, so when you have chosen your dataset, add the topic and the link to [HW7-datasets.md](https://github.com/cs625-datavis-fall19/shared-files/blob/master/HW7-datasets.md) (edit the Master branch and commit). *If someone else has already chosen the dataset you were planning to use, you must choose a different dataset.* For your own benefit, you should choose your dataset no later than Fri, Nov 8.

Note: The charts you produce for HW7 will be considered draft charts.  For HW8, you will choose one of your charts and refine it according to data journalism/storytelling principles.  Spend most of your time for HW7 on the EDA process and developing good questions.

## Report

Your report is an important part of this assignment. I expect your report to include your name, CS625-HW7, date, and appropriate headings and Markdown markup for clarity and neatness. You will lose points if there are many spelling or grammatical errors. 

Your report should contain the following information:
* description of your dataset (including a link to the original source of the data)
* description of your EDA process -- explain the initial questions you asked, describe any statistics or charts created to initially explore the data, and describe how you generated additional questions
* final detailed questions that you arrived at
* images of your sketch or draft charts
* explanations of the charts and how they will be used to answer the detailed questions

If you use R, any code needed to document your EDA process should be runnable and embedded in your RMarkdown report. Make sure to 'Knit' your report to produce Markdown suitable for Github and commit both the .Rmd and .md files to your repo. You may use [template.Rmd](https://github.com/cs625-datavis-fall19/assignments/blob/master/template.Rmd) to get started.

If you use Vega-Lite, your report must include a link to the Observable notebook that contains your Vega-Lite code and charts.

As always, you must include a section titled "References", including links to any examples that you used in completing this assignment.

## Submission
Submit the URL of your report in Blackboard:
* Click on HW7 under Homeworks
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your `report.md` file into the edit box (should be something like https<nolink>://github.com/cs625-datavis-fall19/hw7-questions-*username*/blob/master/report.md)
* Make sure to "Submit" your assignment.
