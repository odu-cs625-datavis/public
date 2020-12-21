# Week 2 Open Refine Tutorial

We will be walking through the tutorial available at http://web.archive.org/web/20190105063215/enipedia.tudelft.nl/wiki/OpenRefine_Tutorial up to the section titled "Exploring the data with scatter plots".

As we go through the tutorial, I will ask you to perform some extra tasks that we'll discuss together.

First, download [university-data.csv](university-data.csv) to your local machine to load into OpenRefine. 

### Load file and create project

**Q1:** *How many rows are in the dataset?*

### Clean up country names

After you choose "Cluster and edit", go to the "# Choices in Cluster" chart and move the left slider over from the edge so that it only shows clusters with more than 1 choice.

As you are examining clusters, you can choose "Browse this cluster" to open up a new window with just the entries in that cluster.

**Q2:** *What other countries had issues with spelling? How did you find them?*

After using clustering to clean up the country names, use a text facet.  In the country column, choose "Facet > Text facet".

**Q3:** *How many different country names are listed?*

Using the "edit" option, fix any remaining country name issues you find. 

**Q4:** *What other countries did you edit using the text facet?*

**Q5:** *How many different country names are now listed?*

Sort the facet by count.

**Q6:** *How many universities are listed for the US?  Does this number make sense?*

We'll investigate this more later.

### Clean up values for the number of students

**Q7:** *After removing the "+", "~", and "," characters from the numStudents column and converting the column to number, how many non-numeric rows are left?*

Don't remove rows that have blank values for numStudents, only those that have non-numeric values.

**Q8:** *After performing the cleaning specified and removing rows that have non-numeric values for numStudents, how many rows are left in the dataset?*

Before we move on, let's examine the range of values in the numStudents column.  

**Q9:** *What is the maximum value in the numStudents column? Does this number make sense?*

**Q10:** *What is the enrollment of the largest university in the world?*

Move the left slider in the numStudents numeric facet to the left so that the values shown are greater than 100,000,000.

Since this dataset came from Wikipedia, use Wikipedia to verify and correct the number of students at the universities that show more than 100 million students.

**Q11:** *What were the universities and what did you update?*

We'll come back to this column later.

### Clean up values for the endowment

**Q12:** *After converting the text to lowercase, how many entries used the term "million" in the endowment column?*

**Q13:** *After converting those with "million" to numeric, how many entries were left with the word "million"?"*

**Q14:** *How many entries used the word "billion"?*

After converting those with "billion" to numeric, convert the whole endowment column to numeric.

**Q15:** *How many non-numeric entries are left in the endowment column?*

Don't delete the rows with non-numeric values yet, but do a bit more work to clean up any values that you can interpret.  

**Q16:** *What operations did you perform and how many non-numeric values are left in the endowment column?*

### Finding issues in other columns

Identify and fix issues you find with university names (including removing URL encoding as described earlier in the tutorial)

**Q17:** *What operations did you perform?*

### Cleaning up dates

For dates, we're just looking in the established column.

**Q18:** *After converting to date and creating the timeline facet, how many of the established dates are non-time values?*

After converting the dates to years, transform the column to numeric.  Then create a numeric filter. Slide the left slider over so that the only values shown are greater than 10,000,000.  Determine the correct values and manually edit these entries.

**Q19:** *What were the universities and what did you update?*

Reset the numeric filter and continue fixing the dates.

**Q20:** *What were the universities and what did you update?*

### Deduplicate entries

**Q21:** *How many rows are remaining in the dataset?*

Now, let's look back at Q6.

**Q22:** *How many universities are listed as in the US?*

Let's also look back at numStudents (Q9-11). Investigate any universities that have more students than the largest university in the world.

**Q23:** *What were the universities and what did you update?*

### Export Data

*Export the cleaned dataset as a CSV*

*Export the commands you used to clean the dataset.  Under the "Undo/Redo" tab, click "Extract..." and save the JSON file.*

## Other Resources

Here are a few other OpenRefine tutorials:
* reproducible data tutorial - https://vickysteeves.gitlab.io/2018-uutah-repro/cleaning-data.html
    * uses same dataset as this tutorial
* tutorial using Raleigh, NC building permits database - https://libjohn.github.io/openrefine/start.html#start
* tutorial featuring Ontario breweries - https://zapier.com/blog/openrefine-guide/
