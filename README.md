# DemogD3
Uses D3 to chart demographics vs health risk factors. 
The chart itself is in an iframe. That website reads the data files and uses D3 to create the graph with three separate scatter plots
within one chart. State abbreviations are displayed within each circle of the scatter plot. A tooltip shows the state's detailed data when the mouse is over a particular circle. As the user switches between the three plots, the axes are redrawn with appropriate scale and the matching data is displayed.


Description

The graph shows three different sets of demographics vs health risks based on 2014 U.S. Census Bureau and the 2014 Behavioral Risk Factor Surveillance System. The three scatter plots are all contained within a single graph, and the user can select any of the x-axes to see the specific data. Data for each U.S. state is plotted, along with details when the user points at a state.

The three sets of data plotted are:

1) Percent living in poverty vs tobacco use
2) Percent who are US-born citizens vs alcohol use (defined as 1 drink in the last 30 days)
3) Percent who are US-born citizens vs seatbelt use.

Sources of Data:
1) From 2014 Census: ACS_14_1YR_B05001 (Nativity and Citizenship Status)
2) From 2014 Census: ACS_14_1YR_S1701 (Poverty Status)
3) From 2014 Behavioral Risk Factor Surveillance System (BRFSS_2014_Overall)

Pre-Analysis:
I analyzied various demographic factors and risk factors from the above data sources, looking at correlations using the Excel 
CORREL function. I decided on the three sets plotted above, because they showed high correlations.


User Instructions

- Select any of the X-Axis labels to see other data.
- Note that the Y-Axis labels are not selectable, but will be bold-faced when their corresponding X-axis is selected.
- Point the mouse at a state, and the details for that state will be displayed in a box until the mouse is moved. This works best when   pointing toward the bottom of the circle.

Analysis

- The poverty demographic and health risk of having at least one alcoholic drink the past 30 days had a correlation of -0.534. This suggests a negative correlation. It appears, in general, that states with wealthier people were more likely to have people who drink alcohol.
- The demographic of US citizens who were born in the US and health risk of using tobacco had a correlation of 0.593. This suggests a positive correlation. States with more people who are US-born citizens are more likely to have more tobacco users.
- The demographic of US citizens who were born in the US and health risk of wearing seatbelts had a correlation of -0.504. This suggests a negative correlation. States with more people who are US-born citizens have a higher incidence of people not wearing seatbelts.
- Note: The percent of US-born citizens in Puerto Rico was derived based on the number of US citizens born either in the US or in Puerto Rico.
