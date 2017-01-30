
#Summary -

You can find the final sketch here: 
http://bl.ocks.org/sbassam/f5bcb52c52c3c1767572e8ba0b88d261



In this project, I'll be improving the first chart, titled "Sector Breakdown of Obama Inauguration Donors" here: 
https://www.opensecrets.org/obama/inaug_2009.php

My final sketch shows the sector breakdown of contributors to Obama's inaguration ceremony in 2009. As you can see, 
each bar is associated with a sector. Next to each bar there is a value that indicates the % of total the sector makes up to. when hovering over each bar, you can see the total value in the little text that comes up. You'll also be able to see a line that's drawn vertically to better compare bars. 
 

NOTE/UPDATE: I happen to work at OpenSecrets.org. Recently, we decided to change the mentioned chart. It used to be a pie chart similar to the one that's currently under it (Top States of Inauguration Donations). 

For many reasons, pie chart is not a good choice (mostly because our eyes aren't good at attributing quantitative value to two dimensional spaces.) I'll be replacing it with a vertical bar chart. 


#Design - explain any design choices you made including changes to the visualization after collecting feedback

##1st iteration (index_V1):

	- started with a simple bar chart. 
	- used default dimple settings. didn't change it much.
	- added title, x label, and y label.

##2nd iteration (index_V2):
Based on the feedback:
	- Changed the bar color. used the color pallette (see ref.)
	- Added %s to the mouse-over interaction. This is probably the most important change since showing proportions of 	the whole is the main message this chart needs to convey.
	- Added "total" to mouse-over interaction. modified to show the exact number instead of showing in millions. 
	- removed the background gridlines as they seemed unnecessary.

###Data processing: To generate the percentages, I had to aggregate the data. I did that using the following lines of code:
'''
// Adding percentage labels
          s1.afterDraw = function (shape, data) {
            var s1 = d3.select(shape),
            rect = {
              x: parseFloat(s1.attr("x")),
              y: parseFloat(s1.attr("y")),
              width: parseFloat(s1.attr("width")),
              height: parseFloat(s1.attr("height"))
            };
// Format the number
                .text(d3.format(",.1f")((data.xValue / sumTotal) * 100) + "%");'''


#Feedback - include all feedback you received from others on your visualization from the first sketch to the final visualization

##1st iteration:
	- liked the use of vertical instead of horizontal
	- disliked the transparency of bars (you can see gridlines through the bars)
	- "when I hover over a bar, it shows the total in m (e.g. 9m) but i'd like to see the exact number"
	- "i'd like to know what percentage of the whole each bar makes up to."

#Resources - list any sources you consulted to create your visualization

1) This data is from Center For Responsive Ploitics (OpenSecrets.org) and is for non-commercial use only.
2) http://dimplejs.org/index.html
3) http://www.storytellingwithdata.com/blog/2011/07/death-to-pie-charts
4) http://flatuicolors.com/
