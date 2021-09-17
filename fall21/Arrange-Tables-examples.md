# Arrange Tables Examples

## Grouped Bar Charts

### Example 1

[Remake: Time Series Column Chart](https://policyviz.com/2018/06/07/remake-time-series-column-chart/), PolicyViz.com, June 2018

|Original Chart | |
|--|:--|
|<img src="https://policyviz.com/wp-content/uploads/2018/06/USDA_Paired_Column_Chart-1024x806.jpg" width=600/>|<b>Q:</b> <i>What's your first observation from this chart?</i><ul><li>Acreage for all 5 crops increased over the time period</li><li>Acreage for Cotton fell in the last year</li></ul>Problems with this chart:<ul><li>too many columns (bars) per category</li><li>each column represents year, which is ordered, so it's not easy to associate year with color hue<br/>(have to keep looking at legend)</li></ul>|

|Remake 1: line chart | |
|--|:--|
|<img src="https://policyviz.com/wp-content/uploads/2018/06/PolicyViz_USDA_Remake_Line_Chart.png" width="400"/>|<ul><li>no legend, label at the end of each line</li><li>reveals <ul><li>Cotton's drop in the last year</li><li>Rice is in the middle of all 5 crops</li></ul></li></ul>|

|Remake 2: small multiples line chart (cycle chart)| |
|--|:--|
|<img src="https://policyviz.com/wp-content/uploads/2018/06/PolicyViz_USDA_Remake_Cycle_Chart.jpg" width="400"/>|<ul><li>small multiples line chart where each crop gets its own panel</li><li>advantage: more space for the graph</li></ul>|

**Q:** *Which do you prefer?*

### Example 2

[Remake: Paired Column Chart from WSJ](https://policyviz.com/2018/03/01/remake-paired-column-chart-from-wsj/), PolicyViz.com, March 2018

|Original Chart | | 
|--|:--|
|<img src="https://policyviz.com/wp-content/uploads/2018/02/OutofWork_ColumnChart_WSJ.jpg" width=600/>|Compare unemployment rates within and between 4 different racial/ethnic groups between 2004-2014.<p>Problems with this chart: too many columns</p>|

|Remake 1: line chart| |
|--|:--|
|<img src="https://policyviz.com/wp-content/uploads/2018/02/PolicyViz_WSJ_Remake_LineChart-1024x613.png" width=400/>|no legend, labels near each line|

|Remake 2: small multiples line chart (cycle chart)| |
|--|:--|
|<img src="https://policyviz.com/wp-content/uploads/2018/02/PolicyViz_WSJ_Remake_SmallMultiples-1024x615.png" width=600/>|added data value for first and last point<br>(makes clear that the unemployment rates for Whites and Asians did not change overall)|

**Q:** *Which do you prefer?*

**Q:** *What other things do you see with either the line chart or cycle chart that are difficult to spot with the bar chart?*

## Stacked Bar Charts

### Example 1

[Remake: Stacked Column Chart from Merrill Lynch](https://policyviz.com/2018/02/22/remake-stacked-column-chart-merrill-lynch/), PolicyViz.com, Feb 2018

|Original Chart| |
|--|:--|
|<img src="https://policyviz.com/wp-content/uploads/2018/01/MerrillLynch_GMLrV6kTe2fq8rHGdbm9ErAxLha7HBJs0qEzFDT0Tqs.jpg" width=600/>|Shows distribution of spending across 7 categories by 4 generations of Americans.<p>Could be changed:</p><ul><li>remove gridlines and vertical axis labels -- since there are labels in each segment</li><li>delete legend and directly label chart</li><li>order the generations by age:  Traditionalists, Baby Boomers, Gen X, Millennials</li><li>lots of colors to look at</li></ul><p>Main points raised in accompanying text:</p><ul><li>"All four groups spend about the same amount of their spending on food."</li><li>"Millennials concentrate more of their spending at restaurants while other 3 spend more at grocery stores."</li><li>"Millennials are spending more of their income on electronics/hobbies/clothing stores than older generations."</li></ul>|

**Q:** *How easy is it to see these points from the original chart?*

|Remake 1: small multiples| |
|--|:--|
|<img src="https://policyviz.com/wp-content/uploads/2018/01/MerrillLynch_BrokenStackedColumnChart.png" width=400/>|<ul><li>breaks the bars and gives each section it's own aligned axis</li><li>highlight just the categories of Restaurants, Groceries, <br/>Electronics/Hobbies/Clothing since those are the ones mentioned in the text</li><li>still a little busy</li></ul>|

|Remake 2: line chart| |
|--|:--|
|<img src="https://policyviz.com/wp-content/uploads/2018/01/MerrillLynch_LineChart.png" width=400/>|<ul><li>age ranges are at least ordered, so this mapping is ok</li><li>can find trends, but can't see part-to-whole relationship</li></ul>|

|Remake 3: pie chart| |
|--|:--|
|<img src="https://policyviz.com/wp-content/uploads/2018/01/MerrillLynch_PieCharts.jpg" width=400/>|<ul><li>focus is on how the 3 segments (Restaurants, Groceries, <br/>Electronics/Hobbies/Clothing) sum to around 50%</li><li>hard to see: How much spending on Restaurants has changed from the Millennial to Traditionalist generation?</li><li>easy to do: Millennials spend more than half of their budget on these three categories while Traditionalists don’t</li></ul>|

Final change - title
* "Consumer Spending by Generation" doesn't illustrate the main point
* “Millennials spend more at restaurants while older generations spend more at grocery stores” -- this is what you want viewers to take away from the chart


### Example 2

[When Are 100% Stacked Bar Graphs Useful?](https://www.perceptualedge.com/blog/?p=2239), Stephen Few's blog, Jan 2016

*Note: The comments section of this blog post contains an interesting conversation between Few and Cole Nussbaumer Knaflic (author of many of the ["storytelling with data"](https://storytellingwithdata.com/blog) blog posts).*

|Original Chart | Re-design|
|--|--|
|<img src="http://www.perceptualedge.com/blog/wp-content/uploads/2016/01/Coles-Graph.png" width=300/>|<img src="http://www.perceptualedge.com/blog/wp-content/uploads/2016/01/Redesign-of-Coles-Graph.png" width=300/>

"When multiple 100% stacked bars appear in a graph, they only provide information about the parts of some whole, never about the wholes and how they differ. Therefore, they would never be appropriate when information about totals and the parts of which they are made are both of interest."

Few's position: "A 100% stacked bar graph never serves as the best solution for a time series. Stacked segments of bars do not display patterns of change through time as clearly as lines."

Nussbaumer Knaflic's position: " I like the intrinsic visual cue of the part-to-whole relationship and in this case think the trade-offs are worth it. *In general, I don’t think there is a single 'right' or 'best' answer when it comes to visualizing data*, rather different scenarios will call for different approaches and different individuals will make different design choices."

**Q:** *How does the 100% stacked bar chart compare to the line chart shown in the article?*

(According to Few) 100% stacked bar graphs are only useful in three specific situations:  

|Examples| |
|--|:--|
|<img src="http://www.perceptualedge.com/blog/wp-content/uploads/2015/08/Womens-Equality-Day-Infographic-Redesigned.jpg" width=300/>|When the bars consist of only two segments (e.g., male and female)|
|<img src="http://www.perceptualedge.com/blog/wp-content/uploads/2016/01/Coles-Other-Graph.png" width=300/>|When we need to compare the sum of multiple parts among multiple bars|
|<img src="http://www.perceptualedge.com/blog/wp-content/uploads/2016/01/Coles-Final-Graph.png" width=300/>|When we need to compare the percentages of responses to Likert scales|

### Example 3

[declutter! (and question default settings)](http://www.storytellingwithdata.com/blog/2019/5/13/declutter-and-question-defaults), storytellingwithdata blog, May 2019

|Original Chart| |
|--|:--|
|<img src="https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1556822166235-ELYVOOA6LZI7XKHEP10C/ke17ZwdGBToddI8pDm48kIAfb53QkaVqzS3DhVYRS6pZw-zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZUJFbgE-7XRK3dMEBRBhUpzyr2Kis3grtr84yTUzrCAKQJH0CQ-rS_YAti8PrP44LSZnEvomOQucCotiiGNAzj4/Picture2.png?format=500w" width=400/>|Shows percentage of babies born with a 24-hour period, broken down by day of the week.|

**Q:** *What things would you change?*

|Re-design| |
|--|:--|
|<img src="https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1556822373043-LCA2E38DALYTKQX53ZDH/image-asset.png?format=500w" wdith=400/>|Author's suggestions to change:<ul><li>remove the chart border</li><li>remove the gridlines</li><li>only use data labels when exact values are important</li><li>thicken the bars - bars should be wider than the white space between them</li><li>title the axes appropriately</li><li>drop unnecessary trailing zeros from y-axis labels</li><li>abbreviate x-axis labels so they can be read horizontally</li><li>move the legend labels next to the data</li><li>reduce the number of colors</li><li>add a takeaway title - what is the main point of the chart?</li></ul> |
