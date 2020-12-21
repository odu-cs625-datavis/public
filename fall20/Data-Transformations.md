# Data Transformations in R In-Class Exercises

The goal of this exercise is to gain experience using the [dplyr package](https://www.rdocumentation.org/packages/dplyr/versions/0.7.8) in R to transform data. This is in preparation for performing EDA and HW6. 

All of these exercises come from [Chapter 5 (Data Transformations)](https://r4ds.had.co.nz/transform.html) in [*R for Data Science*](https://r4ds.had.co.nz)
 
I've set up a [Google Colab R notebook](625_Data_Transformation_R.ipynb) that you can work from.
 
## Exercise

### filter()

[Exercises (5.2.4)](https://r4ds.had.co.nz/transform.html#exercises-8) from [Chapter 5.2](https://r4ds.had.co.nz/transform.html#filter-rows-with-filter)

**Q1.** 1. Find all flights that...

**Q2.** 2. What does `between()` do? Can you use it to simplify the code needed to answer the previous challenges?

### arrange()

[Exercises (5.3.1)](https://r4ds.had.co.nz/transform.html#exercises-9) from [Chapter 5.3](https://r4ds.had.co.nz/transform.html#arrange-rows-with-arrange)

**Q3.** 1. How could you use `arrange()` to sort all missing values to the start? 

**Q4.** 2. Sort `flights` to find the most delayed flights. Find the flights that left earliest.

**Q5.** 3. Sort `flights` to find the fastest flights.

**Q6.** 4. Which flights travelled the longest? Which travelled the shortest?

### select()

[Chapter 5.4](https://r4ds.had.co.nz/transform.html#select)

**Q7.** Use ```select()``` in conjunction with ```arrange()``` to sort by the shortest flight (as above) and move the distance column to the first position. This can be in two commands -- we'll look at using pipes later.

### mutate()

[Exercises (5.5.2)](https://r4ds.had.co.nz/transform.html#exercises-11) from [Chapter 5.5](https://r4ds.had.co.nz/transform.html#add-new-variables-with-mutate)

**Q8.** 1. Currently `dep_time` and `sched_dep_time` are convenient to look at, but hard to compute with because they’re not really continuous numbers. Convert them to a more convenient representation of number of minutes since midnight.

**Q9.** 2. Compare `air_time` with `arr_time - dep_time`. What do you expect to see? What do you see? What do you need to do to fix it?
