# Marks and Channels Tutorial

We're going to explore the use of marks and channels using both Vega-Lite and R, using these tutorials:
* Vega-Lite/Observable tutorial - https://observablehq.com/@uwdata/data-types-graphical-marks-and-visual-encoding-channels
* R tutorial - https://r4ds.had.co.nz/data-visualisation.html 

## Using Vega-Lite/Observable

We'll be following the [Data Types, Graphical Marks, and Visual Encoding Channels](https://observablehq.com/@uwdata/data-types-graphical-marks-and-visual-encoding-channels?collection=@uwdata/visualization-curriculum) tutorial developed by the [Interactive Data Lab](https://idl.cs.washington.edu) at the University of Washington (led by Jeffrey Heer).

The tutorial uses data from [Gapminder](https://www.gapminder.org), so to set the stage, first watch the 4-minute video about this data, "[Hans Rosling's 200 Countries, 200 Years, 4 Minutes](https://www.youtube.com/watch?v=jbkSRLYSojo)".

### Setup
To get started, open the [tutorial](https://observablehq.com/@uwdata/data-types-graphical-marks-and-visual-encoding-channels?collection=@uwdata/visualization-curriculum) and make sure that you're logged into Observable.  Then [create a new Observable notebook](https://observablehq.com/new) in a separate window.

Copy the following into the first cell of the new notebook:

```
md`# Marks and Channels Tutorial Solution

Your Name  
[CS 625, Fall 2019](https://www.cs.odu.edu/~mweigle/CS625-F19/)

Based on walking through the [Data Types, Graphical Marks, and Visual Encoding Channels tutorial]
(https://observablehq.com/@uwdata/data-types-graphical-marks-and-visual-encoding-channels) from IDL`
```

Replace `Your Name` with your name and make sure to put 2 extra spaces after your name so that the CS 625, Fall 2019 line appears on the next line.

Press the triangle (looks like a Play button) at the right corner of the cell to run the code to make sure that it displays properly.  If you want to hide the source and just see the result, click the three dots to the left of the cell and choose 'Close' (if 'Close' isn't an option, you may need to unpin the cell first by clicking the blue pushpin button to the left of the cell).

You'll be copying and pasting code from cells in the tutorial into your notebook.  The best way to do this is to click on the three dots to the left of a cell and choose 'Edit' and then copy the source (shown with a gray background).

To add a new cell, click the plus sign below the previous cell.

The final piece of setup before beginning the tutorial is to copy the two import statements from the tutorial (before the "Global Development Data" header). These will need to be in separate cells.

### Tutorial

For each section of the tutorial that you walk through, you might want to create a subheading in your notebook to keep track.  You can do this with a Markdown cell like

```
md`## Global Development Data`
```

Walk through the **Global Development Data** section and copy the commands into your notebook.  Make sure that you understand what each command is doing and that you end up with the same table of the data from 10 countries in 2000 as shown in the tutorial.

Read through the **Data Types** section and note how their data type definitions map to the ones we discussed last week in Chapter 2.

Next, we'll actually create some charts to explore encoding channels by walking through the **Encoding Channels** section.  Again, make sure that you understand what each piece of code is doing.  If you don't, then ask!

**Encoding Channels > Y** 
* Answer the question in the tutorial *What happens to the chart above if you swap the O and Q field types?* by creating a new cell and performing that swap.  Explain what happened.
* Answer *What happens if you also add nice:false to the scale properties above?* by creating a new cell and making that change.  Explain what happened.

**Encoding Channels > Color and Opacity**
* Create a cell that demonstrates how to set the opacity by passing a default value to the mark* method.

**Encoding Channels > Tooltips and Ordering**
* What does the cluster field represent?

**Encoding Channels > Column and Row Facets**
* This section is getting a bit ahead of ourselves, but it's useful for you to be exposed to the idea of small multiples early on.
* Answer *Can you rewrite the chart above to facet into rows instead of columns?* by creating a new cell and trying it out.  Explain what you did and what happened.

*Skip the **A Peek Ahead: Interactive Filtering** section.*

**Graphical Marks > Bar Marks** 
* Create a new cell and set the rangeStep property of the x channel scale attribute to 12.  Explain what happened.

**Graphical Marks > Line Marks** 
* Create a new cell and change or remove the width value on the line chart.  Explain what happened.
* Create a new cell and adjust the rangeStep on the slope graph. Explain what happened.

**Graphical Marks > Area Marks**
* Answer *What happens if you instead set it normalize?*

*We'll stop with this tutorial after you've answered the question above -- skip `stack(null)` (will just cause confusion for viewers) and the other fancy area mark examples.*

## Using R

We'll follow the [R for Data Science data visualization](https://r4ds.had.co.nz/data-visualisation.html) tutorial.  Since you've already worked through Sections 3.1-3.2 (in HW1), we'll start with [Section 3.3 (Aesthetic mappings)](https://r4ds.had.co.nz/data-visualisation.html#aesthetic-mappings). 

Create a new repo in GitHub for your work and open the project in RStudio (this should be similar to what you did in HW1).  Create a new file in RStudio to work through the tutorial.  You can copy/paste from [template.Rmd](template.Rmd) to get started (make sure to change the title and your name).

### Aesthetic mappings

Work through the examples in [Section 3.3 (Aesthetic mappings)](https://r4ds.had.co.nz/data-visualisation.html#aesthetic-mappings) and answer the questions in the **Exercises** section.

### Facets

Work through the examples in [Section 3.5 (Facets)](https://r4ds.had.co.nz/data-visualisation.html#facets), but *skip the exercises*.

### Geometric objects

*Skip the Geometric objects section*

### Statistical transformations
Work through the examples in [Section 3.7 (Statistical transformations)](https://r4ds.had.co.nz/data-visualisation.html#statistical-transformations) through the bar chart of proportion example, then *skip the the rest of this section (including the exercises).*

Note that the bar charts with derived counts on the y-axis (generated with `geom_bar()`) are really histograms rather than standard bar charts (which can be generated with `geom_col()`).  We'll look at the differences between again this semester.

Note that to map a channel to a computed variable, like prop, it needs to be between `..` characters, like `..prop..`.

### Position adjustments
Work through the examples in [Section 3.8 (Position adjustments)](https://r4ds.had.co.nz/data-visualisation.html#position-adjustments)  (through the `position="dodge"` example but *skipping the `position="identity"` example and the exercises*).

Note that using `position="dodge"` creates a grouped bar chart instead of a stacked bar chart.

### Additional R Examples

For the rest of this tutorial, we'll look at some features to help replicate some of the charts we did in the Vega-Lite tutorial.

**Chart options**

To make these look as much like the Vega-Lite charts, we're going to change the default color of marks from black to "steelblue" (`color="steelblue"`) and change the default theme (`theme_bw()`) to generate a white background and black foreground. For the scatterplot below, we also change the stroke width, shape (to open circle), and force the origin to be a (0,0).

First, let's create a scatterplot that looks similar to the Vega-Lite scatterplots.

```
ggplot(data = mpg) + 
  geom_point(mapping = aes(x=cty, y=hwy), 
             color="steelblue", stroke=0.75, shape=1) + 
  theme_bw() + xlim(0, NA) + ylim (0, NA)
```

**Bar chart**

We're going to look at a different dataset named `msleep`. This dataset looks at the sleeping habits of various mammals.  Preview the dataset with `msleep`.

To create a standard bar chart instead of histogram, we'll use `geom_col()` instead of `geom_bar()`.  Run the command `?geom_bar` in R to read about the differences between the two.

In addition to standard barchart variables, we are removing the vertical grid lines so the chart isn't so cluttered.

For this chart, we're going to save the base chart as `barp` so that we can just add to it as we go along.

```
barp <- ggplot(data = msleep) + 
  geom_col(mapping = aes(x=name, y=sleep_total), fill="steelblue") + 
  theme_bw() +    
  theme(panel.grid.major.x = element_blank(),
        panel.grid.major.y = element_line(size=.1, color="black"))
barp
```

Yes, this is unreadable, so we can rotate the x-axis labels.

```
barp + theme(axis.text.x = element_text(angle = 90, hjust = 1))
```

**Horizontal bar chart**

Another option is to flip the plot to use horizontal bars using `coord_flip()`.  Note that we need to change which grid lines are removed. This is a little better, but more work can be done (later) to spread the y-axis labels out.

```
barp + coord_flip() +  
  theme(panel.grid.major.x = element_line(size=.1, color="black"),
        panel.grid.major.y = element_blank())
```
