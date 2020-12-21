# Storytelling In-Class Tutorial/Exercises 

In this set of exercises, we'll review methods to add annotations and layers to charts in R and Vega-Lite. 
 
## Part A - Annotations in R Tutorial/Exercises

"To help others quickly build up a good mental model of the data, you will need to invest considerable effort in making your plots as self-explanatory as possible."

These are some notes to review from [Chapter 28 (Graphics for Communication)](https://r4ds.had.co.nz/graphics-for-communication.html) in [*R for Data Science*](https://r4ds.had.co.nz). We'll work breakout exercises for "Annotations" and "Scales".  I've set up a [Google Colab notebook for these exercises](625_Storytelling_in_R_exercise.ipynb) that you can copy.

### [28.2 Label](https://r4ds.had.co.nz/graphics-for-communication.html#label)
* adding title, subtitle, caption
* changing axes labels, legend title

`labs()` - can add title, subtitle, caption, x/y axis titles, legend title

### [28.3 Annotations](https://r4ds.had.co.nz/graphics-for-communication.html#annotations)

* label aesthetic 

`geom_text()` - similar to `geom_point()`, but has the additional aesthetic `label`

`geom_label()` - draws a rectangle behind the text

`ggrepel::geom_label_repel()` -- non-overlapping labels

* turn off legend to directly label plot

`theme(legend.position = "none")`

* add single headline to chart

* annotation layer (*only mentioned in the exercises*)

`annotate()` - see https://ggplot2.tidyverse.org/reference/annotate.html

**[Breakout Exercises](https://r4ds.had.co.nz/graphics-for-communication.html#exercises-75)**

### [28.4 Scales](https://r4ds.had.co.nz/graphics-for-communication.html#scales)

* Note the naming scheme for scales: `scale_` followed by the name of the aesthetic, then `_`, then the name of the scale.

Ex: `scale_x_continuous()`, `scale_y_continuous()`, `scale_colour_discrete()`

* axis ticks

`breaks` - controls the position of the ticks, or the values associated with the keys

`labels` - controls the text label associated with each tick/key

Another use of `breaks` is when you have relatively few data points and want to highlight exactly where the observations occur. See the presidential example at the end of [Section 28.4.1](https://r4ds.had.co.nz/graphics-for-communication.html#axis-ticks-and-legend-keys).

* legend layout

`theme(legend.postion =` {"left", "top", "bottom", "right" (default)}

* replacing a scale on axis and colors

`scale_colour_brewer()` - set the color scale, uses the RColorBrewer package, set of scales shown at https://r4ds.had.co.nz/graphics-for-communication.html#fig:brewer

`scale_colour_manual()` - set manual colors

**[Breakout Exercises](https://r4ds.had.co.nz/graphics-for-communication.html#exercises-76)**

### [28.5 Zooming](https://r4ds.had.co.nz/graphics-for-communication.html#zooming)

* share scales over multiple plots (similar to what's done in small multiples)

Using `limits` to share scales among multiple plots.

### [28.6 Themes](https://r4ds.had.co.nz/graphics-for-communication.html#themes)

`theme_gray()` - default

There are several others available, shown at https://r4ds.had.co.nz/graphics-for-communication.html#fig:themes

### [28.7 Saving your plots](https://r4ds.had.co.nz/graphics-for-communication.html#saving-your-plots)

Saving images and changing the size

## Part B - Annotations in Vega-Lite Examples

Here are several examples of adding annotations to charts in Vega-Lite.  I've put them in a single Observable notebook so that we can edit them.

https://observablehq.com/@weiglemc/cs-625-vega-lite-annotations-examples

Links here are to the original examples from the Vega-Lite documentation
* [Simple Bar Chart with data label at end of bar](https://vega.github.io/vega-lite/examples/layer_bar_labels.html)
* [Layering text over heatmap](https://vega.github.io/vega-lite/examples/layer_text_heatmap.html)
* [Line charts with labels near lines](https://vega.github.io/vega-lite/examples/layer_line_co2_concentration.html)
* [Horizontal mean line overlay on bar chart](https://vega.github.io/vega-lite/examples/layer_precipitation_mean.html)
* [Vertical mean line overlay on histogram](https://vega.github.io/vega-lite/examples/layer_histogram_global_mean.html)
* [Line chart with highlighted rectangles](https://vega.github.io/vega-lite/examples/layer_falkensee.html)
