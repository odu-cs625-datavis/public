# Homework 2: Data Cleaning 

**Due:** Thursday, September 22, 2022 by 11:59pm 

The goal of this week's assignment is to gain experience using OpenRefine for data cleaning.  

**Note:** This assignment assumes that you have already downloaded and installed [OpenRefine](https://openrefine.org) and worked through the OpenRefine tutorial from Week 2 of CS 625.

## Assignment

Write a report that describes how you carried out the tasks in Part 1 and how you arrived at the answers to the questions in Part 2.

### Report
For this assignment, since you'll just be describing the actions you took using OpenRefine without including R code, you can either directly write in Markdown in `report.md` or your can use R Markdown in `report.Rmd` and the Knit process to generate your `report.md`. (In any case, `report.md` is the file that I will use for grading.)

I have not provided a template, but I expect your report to include your name, CS625-HW2, date, and appropriate headings and Markdown markup for clarity and neatness. You will lose points if there are many spelling/grammatical errors or your report is hard to read because of formatting issues.

As for all reports, there should be a "References" section that includes links to any examples that you used in completing this assignment.

### Part 1. Data Cleaning

Create a new project in OpenRefine and load the PetNames.tsv dataset available from https://github.com/jgolbeck/petnames (read the README.txt in that repo for more information on the dataset).  If you view the raw version of the data file in GitHub, you can copy that URL directly into OpenRefine to load the data without downloading it separately.

Use OpenRefine to clean the dataset of pet names so that you can answer the questions in Part 2.  Make sure to keep track of all operations you perform. As much as you can, use OpenRefine facets and GREL transforms to clean the data rather than manual editing (though, some cleaning will need to be done manually). 

There are a couple entries where multiple pets are in the same entry. Make a decision on how to handle these cases and document it in your report.

*Caution:* This is a large, messy dataset.  Clean the data as well as you can, with an eye towards being able to answer the questions in Part 2, but you are not expected to fully clean the entire dataset.

In your report, explain the steps you took to clean the data. Include screenshots, GREL statements, etc. as needed to clearly document what you did. If you did any manual cleaning, note that and explain why you did this manually. Include enough detail so that I am convinced that you understand how to use OpenRefine. 

You will likely not have learned everything in class that you need to know to complete the assignment. I expect that you will watch the tutorials and read documentation, including documentation on the [GREL regex language](https://docs.openrefine.org/manual/expressions#grel-general-refine-expression-language).

When you are done cleaning the file:
* Export the file as a new CSV and save it in your repo as `HW2-petnames.csv`.
* Extract JSON scripts containing all of the operations you performed on the file and save it in your repo as `HW2-petnames.json`. (Select **Extract** at the top of the **Undo/Redo** tab. Then copy and paste the JSON script into a new file.)

### Part 2. Analyze Cleaned Data

Use the cleaned data to answer the following questions in your report (and explain how you arrived at the answers):
1. How many types (kinds) of pets are there?
1. How many dogs? 
1. How many breeds of dogs?
1. What's the most popular dog breed?
1. What's the age range of the dogs?
1. What's the age range of the guinea pigs?
1. What is the oldest pet?
1. Which are more popular, betta fish or goldfish? How many of each?
1. What's the most popular everyday name for a cat?
1. What's the most popular full name for a dog?

*I do not expect everyone to have the exact same answers. Some of these will depend upon decisions you make while cleaning the data. Make sure to note any cleaning decisions you made that could have an impact on your answers.*

## Submission
Your GitHub repository should contain the following files (in addition to any assignment files that were provided):
* `report.md` - your report
* `HW2-petnames.csv` - cleaned CSV
* `HW2-petnames.json` - operations used to clean the data in JSON format

Submit the URL of your report (*not the URL of your repo*) in Canvas. Make sure that you have committed and pushed your local repo to GitHub.  Include "Ready to grade @Faryaneh @Kritikagarg" in your final commit message. 

* Click on HW2 under Week 2 in Canvas
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your `report.md` file into the edit box (should be something like https<nolink>://github.com/odu-cs625-datavis/fall22-hw2-*username*/blob/master/report.md)
* Make sure to "Submit" your assignment.
