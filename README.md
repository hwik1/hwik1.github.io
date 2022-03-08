# Belly Button Biodiversity
Module 12 challenge prepared by Hannah Wikum - March 2022
___
## Resources
Data Source: samples.json (provided)

Software: JavaScript, Plotly, HTML, Visual Studio Code
___
## Overview
This project was created to build an interactive visual model of the results of a study on the bacteria found in belly buttons. For each anonymous participant ID, I was given basic demographic information, including how frequently the participant scrubbed his or her navel, as well as the bacterial IDs, names, and values.

Code was provided to filter for various participant IDs and display the related demographic information. To represent the remaining data, I made a number of charts for the webpage using Plotly:

 1. **Horizontal Bar Graph**
 I used slicing to get the OTU IDs with the top 10 highest sample values, converted those to a string using map, and then used .reverse() to get descending order. Those were added to a horizontal bar chart showing the top 10 OTU IDs that updates whenever the user changes the participant ID.
 
 2. **Bubble Chart**
 Using similar information to the bar graph, I used all sample IDs and values to make a bubble chart that shows how much of each OTU ID was discovered in each sample. You can hover over the bubble for a text box with the OTU ID, sample value, and bacteria names. It is color coordinated by OTU ID and the size of each bubble represents the amount of sample discovered.
 
 3. **Gauge Chart**
 This chart shows how frequently the participant washes his or her belly button on a weekly basis on a scale of zero to ten times. It is color-coded in increments of two to show a preference for washing more frequently (red for less frequently up to green for most frequently). The number of times displays below the chart and the black bar also shows the frequency on the gauge.
___
## Customizations
After creating my interactive webpage, I added a number of customizations to enhance the information:
 
 * Added a background picture on the jumbotron of a navel to offer a quick representation of the subject matter
 * Changed the default font for text on the page to 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif (Note: didn't apply to the text within the charts)
 * Changed the color of the title to red
 * Added a paragraph detailing the background with title, color, and bold formatting
