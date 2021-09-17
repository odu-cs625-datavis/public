# Arrange Tables Examples

## Grouped Bar Charts

#### Example 1 - [Remake: Time Series Column Chart](https://policyviz.com/2018/06/07/remake-time-series-column-chart/), PolicyViz.com, June 2018

<a href="https://policyviz.com/wp-content/uploads/2018/06/USDA_Paired_Column_Chart-1024x806.jpg"><img src="https://policyviz.com/wp-content/uploads/2018/06/USDA_Paired_Column_Chart-1024x806.jpg" height=300/></a>

**Q:** *What's your first observation from this chart?*

1. Acreage for all 5 crops increased over the time period
1. Acreage for Cotton fell in the last year 

Problems with this chart:
* too many columns (bars) per category
* each column represents year, which is ordered, so it's not easy to associate year with color hue (have to keep looking at legend)

Remake 1: line chart
* no legend, label at the end of each line
* reveals
  * Cotton's drop in the last year
  * Rice is in the middle of all 5 crops

Remake 2: cycle chart
* small multiples line chart where each crop gets its own panel
* advantage: more space for the graph

**Q:** *Which do you prefer?*

#### Example 2 - [Remake: Paired Column Chart from WSJ](https://policyviz.com/2018/03/01/remake-paired-column-chart-from-wsj/), PolicyViz.com, March 2018

<a href="https://policyviz.com/wp-content/uploads/2018/02/OutofWork_ColumnChart_WSJ.jpg"><img src="https://policyviz.com/wp-content/uploads/2018/02/OutofWork_ColumnChart_WSJ.jpg" height=300/></a>

Compare unemployment rates within and between 4 different racial/ethnic groups between 2004-2014.

Problems with this chart:
* too many columns

Remake 1: line chart
* no legend, labels near each line

Remake 2: cycle chart
* added data value for first and last point - makes clear that the unemployment rates for Whites and Asians did not change overall

**Q:** *Which do you prefer?*

**Q:** *What other things do you see with either the line chart or cycle chart that are difficult to spot with the bar chart?*

## Stacked Bar Charts

#### Example 1 - [Remake: Stacked Column Chart from Merrill Lynch](https://policyviz.com/2018/02/22/remake-stacked-column-chart-merrill-lynch/), PolicyViz.com, Feb 2018

<a href="https://policyviz.com/wp-content/uploads/2018/01/MerrillLynch_GMLrV6kTe2fq8rHGdbm9ErAxLha7HBJs0qEzFDT0Tqs.jpg"><img src="https://policyviz.com/wp-content/uploads/2018/01/MerrillLynch_GMLrV6kTe2fq8rHGdbm9ErAxLha7HBJs0qEzFDT0Tqs.jpg" height=300/></a>

Shows distribution of spending across 7 categories by 4 generations of Americans.

Could be changed:
* remove gridlines and vertical axis labels -- since there are labels in each segment
* delete legend and directly label chart
* order the generations by age:  Traditionalists, Baby Boomers, Gen X, Millennials
* lots of colors to look at

Main points raised in accompanying text:
* "All four groups spend about the same amount of their spending on food."
* "Millennials concentrate more of their spending at restaurants while other 3 spend more at grocery stores."
* "Millennials are spending more of their income on electronics/hobbies/clothing stores than older generations."

**Q:** *How easy is it to see these points from the original chart?*

Other things to change:
* highlight just the categories of Restaurants, Groceries, Electronics/Hobbies/Clothing since those are the ones mentioned in the text
* added a 50% and 100% gridline to illustrate that those 3 categories sum to just more than 50% for Millineals and just about 50% for Baby Boomers and Traditionalists

Remake 1: small multiples
* breaks the bars and gives each section it's own aligned axis
* still a little busy

Remake 2: line chart
* age ranges are at least ordered, so this mapping is ok
* can find trends, but can't see part-to-whole relationship

Remake 3: pie chart
* focus is on how the 3 segments (Restaurants, Groceries, Electronics/Hobbies/Clothing) sum to around 50%
* hard to see: How much spending on Restaurants has changed from the Millennial to Traditionalist generation?
* easy to do: Millennials spend more than half of their budget on these three categories while Traditionalists don’t

Final change - title
* "Consumer Spending by Generation" doesn't illustrate the main point
* “Millennials spend more at restaurants while older generations spend more at grocery stores” -- this is what you want viewers to take away from the chart


#### Example 2 - [When Are 100% Stacked Bar Graphs Useful?](https://www.perceptualedge.com/blog/?p=2239), Stephen Few's blog, Jan 2016

*Note: The comments section of this blog post contains an interesting conversation between Few and Cole Nussbaumer Knaflic (author of many of the ["storytelling with data"](https://storytellingwithdata.com/blog) blog posts).*

<a href="http://www.perceptualedge.com/blog/wp-content/uploads/2016/01/Coles-Graph.png"><img src="http://www.perceptualedge.com/blog/wp-content/uploads/2016/01/Coles-Graph.png" height=300/></a>

"When multiple 100% stacked bars appear in a graph, they only provide information about the parts of some whole, never about the wholes and how they differ. Therefore, they would never be appropriate when information about totals and the parts of which they are made are both of interest."

Few's position: "A 100% stacked bar graph never serves as the best solution for a time series. Stacked segments of bars do not display patterns of change through time as clearly as lines."

Nussbaumer Knaflic's position: " I like the intrinsic visual cue of the part-to-whole relationship and in this case think the trade-offs are worth it. *In general, I don’t think there is a single 'right' or 'best' answer when it comes to visualizing data*, rather different scenarios will call for different approaches and different individuals will make different design choices."

**Q:** *How does the 100% stacked bar chart compare to the line chart shown in the article?*

(According to Few) 100% stacked bar graphs are only useful in three specific situations:  
* When the bars consist of only two segments (e.g., male and female)
* When we need to compare the sum of multiple parts among multiple bars
* When we need to compare the percentages of responses to Likert scales

#### Example 3 - [declutter! (and question default settings)](http://www.storytellingwithdata.com/blog/2019/5/13/declutter-and-question-defaults), storytellingwithdata blog, May 2019

<a href="https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1556822166235-ELYVOOA6LZI7XKHEP10C/ke17ZwdGBToddI8pDm48kIAfb53QkaVqzS3DhVYRS6pZw-zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZUJFbgE-7XRK3dMEBRBhUpzyr2Kis3grtr84yTUzrCAKQJH0CQ-rS_YAti8PrP44LSZnEvomOQucCotiiGNAzj4/Picture2.png?format=500w"><img src="https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1556822166235-ELYVOOA6LZI7XKHEP10C/ke17ZwdGBToddI8pDm48kIAfb53QkaVqzS3DhVYRS6pZw-zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZUJFbgE-7XRK3dMEBRBhUpzyr2Kis3grtr84yTUzrCAKQJH0CQ-rS_YAti8PrP44LSZnEvomOQucCotiiGNAzj4/Picture2.png?format=500w" height=300/></a>

Shows percentage of babies born with a 24-hour period, broken down by day of the week.  

**Q:** *What things would you change?*

Author's suggestions to change:
* remove the chart border
* remove the gridlines
* only use data labels when exact values are important
* thicken the bars - bars should be wider than the white space between them
* title the axes appropriately
* drop unnecessary trailing zeros from y-axis labels
* abbreviate x-axis labels so they can be read horizontally
* move the legend labels next to the data
* reduce the number of colors
* add a takeaway title - what is the main point of the chart?
