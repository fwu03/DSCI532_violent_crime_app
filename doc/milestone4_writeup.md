Milestone 4 Writeup
================

### Final Improvements

This week we focussed fixing a few bugs and making it easier for users to enter inputs and view charts.

##### Updated User Interface

We made some changes to the user interface that make our app easier to use. We have changed the ordering of the user inputs on the sidebar panel. There are two inputs, cities and crime type, that are used to filter data for both plots. Since these are global settings, it made sense to us to move these up to the top of the page. The last two inputs are the range of years for line chart and a single year for the bar chart. We have added dynamic filtering so that the year for the bar chart is restricted to the range of years in the line chart.

##### Updated Design and Layout

We added a dark navigation bar to the top of our app that contains the title of our app and two tabs. In our old layout, the title was at the top of the page, and the tabs for Plot and Data were below next to the charts. This seemed a little confusing since the tabs were very close to the plot titles. We feel it makes sense to move them away from the plots and next to the title. Further, the black bar makes it clearly differentiates the title of the app from the title of the plots. We have also added a separater between the two plots since before the labels from the top chart were very close to the title of the bottom chart.

##### Changes to the Plots: Colour Scheme and Labels

We made another change to the colour scheme this week. The old colour scheme used a bright yellow colour in the line chart that was difficult to see. We changed the colour scheme so that yellow is no longer used. This makes the chart easier to read.

We also removed some of the axis and legend labels since it was clear what was being listed. In the legend for the line chart, we removed the label "Cities"; and in the legend for the bar chart, we removed the label "Type". Previously, the legend titles were cluttering the design because they were positioned close to the title. Removing them makes the charts cleaner and easier to read.

##### Some Bug Fixes

Previously there was an issue of an error message appearing when no cities were selected. We have now added a message that says "Please select at least one city" when no cities are selected. The error message made it seem like the app crashed, so catching the error and adding a message makes it clear the users that they just need to enter some inputs to continue using the app.

There was also a small issue with the Data tab that we resolved this week. The menu to select the number of entries to view on one screen had four options, but after a selection was made, one of the options was missing. We have fixed this so that users can always select between viewing 10, 30, 50, or 100 entries.

### Remaining Issues and Challenges

##### Remaining Issues We Didn't Fix

-   When a small range of years is selected (i.e.&lt; 3), the labels of the x-axis on the line chart are not integers. Ideally, the axis labels should still be integer values.
-   When data are not available for a particular city, the city shows up in the legend, but not in the line chart. For example, national averages are only available for homicide and total violent crime. When "National" is selected as one of the cities and another type of crime is selected, "National" shows up in the legend, but there is nothing on the plot. We would like to have a small message explaining that data are not available in these cases.

##### Challenges