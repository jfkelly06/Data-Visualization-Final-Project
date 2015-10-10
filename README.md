# Data-Vizualization Final Project
Data visualization using Dimple.js
Data Visualization Final Project
##Summary: 
For this project I intend to analyze historical MLB batting statistics to see what features may be correlated with home run power. I will conduct my analysis in R and generate several exploratory plots there using ggplot2. Once I'm satisfied with the chart, I will work in Dimple.js, to iterate on the chart until I’ve created a visualization that conveys the information in an interesting way!

##Design:
After conducting the data exploration in R, I decided to construct a scatterplot that depicts home run count on the y-axis, and player body mass index (BMI) on the x-axis. Home runs are log normally distributed, so they were rescaled in the final visualization. The trend between the two variables is weak, but non-zero. To better illustrate the relationship, I added a linear trend line. I also included a visual encoding for handedness, which is illustrated by bubble color. Batting average information was also included, and can be viewed by scrolling over data points. 

##Feedback:
###Questions:
•	What do you notice in the visualization?

•	What relationships do you notice?

•	What is the main message?

•	Is there something you do not understand about the graphic or areas of improvement?

1.	The chart is way overpotted. Can you reduce the size of the bubbles and adjust the opacity? Interesting visualization, but there does not appear to be much relationship between the two variables. Is there any way you can add a trend line to illustrate the impact of BMI on home runs? 

  a.	I adjusted the opacity and reduced the size of each bubble. Using R, calculated a regression formula for log10HR and BMI. I then created a new variable and for the linear model (titles “lm”) and I tried to plot it. I ran into considerable difficulty and elected to not include it in the final plot. It’s unfortunate that Dimple does not have native functionality for a regression line!

2.	Very cool visualization! I like that this is interactive, it definitely conveys more information than you get in other tools like Excel. The text is a little bland though; can you add more descriptive labels? It’s a little tough to tell, but it looks like left handed hitters tend to have more home run power!

  a.	I’ve updated the labels and used some CSS styling to make the headline a bit more aesthetically pleasing.

3.	I like this chart quite a bit. It may be a bit overwhelming for some viewers since it conveys a lot of information. You may want to consider removing some of the visual encodings or variables to simplify the chart a bit. Also it the vertical lines are a bit odd, but it makes sense given that some of the BMI measurements were rounded.

  a.	I considered removing batting average, but ultimately decided to keep it in there since other interviewees did not take issue with all the information that is displayed. 
 
##Resources:
•	http://dimplejs.org/examples_index.html

•	Udacity discussion forums

•	Stackoverflow.com

•	Various Github repositories

