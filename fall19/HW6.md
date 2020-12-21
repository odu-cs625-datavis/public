# Homework 6: Data Exploration in R

*This is the public posting of the assignment. See Piazza for the invite link to make your submission in your own repository in the class organization.*

**Due:** November 5, 2019 *before* 9:30am  

The goal of this assignment is to practice exploratory data analysis using R.

## Assignment

The questions and exercises this week come from [Chapter 5 (Data Transformations)](https://r4ds.had.co.nz/transform.html) and [Chapter 7 (Exploratory Data Analysis)](https://r4ds.had.co.nz/exploratory-data-analysis.html) in [*R for Data Science*](https://r4ds.had.co.nz).

Make sure that you click the links provided to view the questions in the book as some include additional information or figures than what is given below.

Before starting this assignment, you will want to complete the [Data Transformations in-class assignment](https://github.com/cs625-datavis-fall19/assignments/blob/master/Data-Transformations.md) as Part A follows directly from the sections in Chapter 5 covered in that exercise.

*There are a total of 15 questions.  Many of these will require significant thought to complete. Do not wait until the last minute to start.*

### Part A - Chapter 5

[Section 5.6.7](https://r4ds.had.co.nz/transform.html#exercises-11)

1. Q4: Look at the number of cancelled flights per day. Is there a pattern? Is the proportion of cancelled flights related to the average delay?

[Section 5.7.1](https://r4ds.had.co.nz/transform.html#exercises-12)

2. Q2: Which plane (`tailnum`) has the worst on-time record?

3. Q3: What time of day should you fly if you want to avoid delays as much as possible?

4. Q4: For each destination, compute the total minutes of delay. For each flight, compute the proportion of the total delay for its destination.

### Part B - Chapter 7

[Section 7.3.4](https://r4ds.had.co.nz/exploratory-data-analysis.html#exercises-13)

1. Q1: Explore the distribution of each of the `x`, `y`, and `z` variables in `diamonds`. What do you learn? Think about a diamond and how you might decide which dimension is the length, width, and depth.

2. Q2: Explore the distribution of `price`. Do you discover anything unusual or surprising? (Hint: Carefully think about the `binwidth` and make sure you try a wide range of values.)

3. Q3: How many diamonds are 0.99 carat? How many are 1 carat? What do you think is the cause of the difference?

[Section 7.5.1.1](https://r4ds.had.co.nz/exploratory-data-analysis.html#exercises-15)

4. Q2: What variable in the diamonds dataset is most important for predicting the price of a diamond? How is that variable correlated with cut? Why does the combination of those two relationships lead to lower quality diamonds being more expensive?

**Extra credit:** Q3: Install the `ggstance` package, and create a horizontal boxplot. How does this compare to using `coord_flip()`?

[Section 7.5.2.1](https://r4ds.had.co.nz/exploratory-data-analysis.html#exercises-16)

5. Q1: How could you rescale the count dataset above to more clearly show the distribution of cut within colour, or colour within cut?

6. Q2: Use `geom_tile()` together with dplyr to explore how average flight delays vary by destination and month of year. What makes the plot difficult to read? How could you improve it?

[Section 7.5.3.1](https://r4ds.had.co.nz/exploratory-data-analysis.html#exercises-17)

7. Q1: Instead of summarising the conditional distribution with a boxplot, you could use a frequency polygon. What do you need to consider when using `cut_width()` vs `cut_number()`? How does that impact a visualisation of the 2d distribution of `carat` and `price`?

8. Q2: Visualise the distribution of carat, partitioned by price.

9. Q3: How does the price distribution of very large diamonds compare to small diamonds? Is it as you expect, or does it surprise you?

10. Q4: Combine two of the techniques you’ve learned to visualise the combined distribution of cut, carat, and price.

11. Q5: Two dimensional plots reveal outliers that are not visible in one dimensional plots. For example, some points in the plot below have an unusual combination of `x` and `y` values, which makes the points outliers even though their x and y values appear normal when examined separately. ... Why is a scatterplot a better display than a binned plot for this case?

## Report

Your report is an important part of this assignment. I expect your report to include your name, CS625-HW6, date, and appropriate headings and Markdown markup for clarity and neatness. You will lose points if there are many spelling or grammatical errors. 

Answer each of the questions using RMarkdown. Any R code needed to answer the questions should be runnable and embedded in your report. Make sure to 'Knit' your report to produce Markdown suitable for Github and commit both the .Rmd and .md files to your repo. You may use [template.Rmd](https://github.com/cs625-datavis-fall19/assignments/blob/master/template.Rmd) to get started.

As always, you must include a section titled "References", including links to any examples (other than [*R for Data Science*](https://r4ds.had.co.nz)) that you used in completing this assignment.

## Submission
Submit the URL of your report in Blackboard:
* Click on HW6 under Homeworks
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your `report.md` file into the edit box (should be something like https<nolink>://github.com/cs625-datavis-fall19/hw6-explore-*username*/blob/master/report.md)
* Make sure to "Submit" your assignment.
