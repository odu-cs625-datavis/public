# Homework 2: Data Cleaning

*This is the public posting of the assignment. See Piazza for the invite link to make your submission in your own repository in the class organization.*

**Due:** September 10, 2019 *before* 9:30am

The goal of this week's assignment is to gain experience using OpenRefine for data cleaning.  

## Setup
This assignment assumes that you have already downloaded and installed OpenRefine and worked through the tutorial from Week 2 of CS 625.

Create a new project in OpenRefine and load the PetNames.tsv dataset available from https://github.com/jgolbeck/petnames (read the README.txt in that repo for more information on the dataset).  If you view the raw version of the data file in GitHub, you can copy that URL directly into OpenRefine to load the data without downloading it separately.

## Assignment

**Note:** In class you will likely not have learned everything you need to know to complete the assignment. I expect that you will watch the tutorials and read documentation, including documentation on the [GREL regex language](https://github.com/OpenRefine/OpenRefine/wiki/General-Refine-Expression-Language).

Use OpenRefine to clean the dataset of pet names so that you can answer the questions below.  Make sure to keep track of all operations you perform. As much as you can, use OpenRefine facets and GREL transforms to clean the data rather than manual editing (though, some cleaning will need to be done manually).

There are a couple entries where multiple pets are in the same entry. For *extra credit*, construct operations to split each pet's information into separate rows. For regular credit, just truncate those rows so that only one pet is counted.

When you are done cleaning the file:
* Export the file as a new CSV and save it in your repo as `HW2-petnames.csv`.
* Extract JSON scripts containing all of the operations you performed on the file and save it in your repo as `HW2-petnames.json`. (Select **Extract** at the top of the **Undo/Redo** tab. Then copy and paste the JSON script into a new file.)

In your report, answer the following questions using the cleaned data:
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

*I do not expect everyone to have the exact same answers. Some of these will depend upon decisions you make while cleaning the data. Make sure to note any decisions you make that could have an impact on your answers.*

## Report
For this project, since you'll just be describing the actions you took using OpenRefine without including R code, you can either directly write in Markdown in `report.md` or your can use R Markdown in `report.Rmd` and the Knit process to generate your `report.md`. (In any case, `report.md` is the file that I will use for grading.)

In your report, explain the steps you took to clean the data. Make sure to include and explain all GREL functions that you used. If you did any manual cleaning, note that and explain why you did this manually.

In answering the questions, also explain how you arrived at the answer using OpenRefine.

**Important:** Your report is the most important part of this assignment. You need to include enough detail so that I am convinced that you understand how to use OpenRefine. I have not provided a template, but I expect your report to include your name, CS625-HW2, date, and appropriate headings and Markdown markup for clarity and neatness. In addition, you will lose points if there are many spelling or grammatical errors. 

### References
Include links to any examples that you used in completing this assignment, including the tutorial examples have been provided.

## Submission
Your GitHub repository should contain the following files (in addition to any assignment files that were provided):
* `report.md` - your report
* `HW2-petnames.csv` - cleaned CSV
* `HW2-petnames.json` - operations used to clean the data in JSON format

Submit the URL of your report (*not the URL of your repo*) in Blackboard:
* Click on HW2 under Homeworks
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your `report.md` file into the edit box (should be something like https<nolink>://github.com/cs625-datavis-fall19/hw2-cleaning-*username*/blob/master/report.md)
* Make sure to "Submit" your assignment.
