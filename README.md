
##Summary -


https://www.opensecrets.org/obama/inaug_2009.php

In this project, I'll be improving the first chart on the above page, titled "Sector Breakdown of Obama Inauguration Donors." 

For many reasons, pie chart is not a good choice (most )

NOTE/UPDATE: I happen to work at OpenSecrets.org. Recently, we decided to change the mentioned chart. It used to be a pie chart similar to the one that's currently under it (Top States of Inauguration Donations). 



##Design - explain any design choices you made including changes to the visualization after collecting feedback
from https://github.com/PMSI-AlignAlytics/dimple/wiki/dimple.chart#addLogAxis

 Log axes are excellent for comparing trends of small and large series, however use with care, they can create charts which are misleading at first glance particularly if used with **stacked series**.

 also, https://eagereyes.org/techniques/stacked-bars-are-the-worst

WHAT IS WRONG WITH THE CURRENT PLOT?
	-- it's a stack bar, it's supposed to show the total but when hovering, it only shows each stack's value.
	-- gradient color
	-- bad colors
	-- a lot of extra elements such as the grid background



##Feedback - include all feedback you received from others on your visualization from the first sketch to the final visualization


PLOT 1 stacked bar 
PLOT 2 stacke bar - log scale
PLOT 3 area chart
PLOT 4 area chart - log scale
PLOT 5 bar chart 
PLOT 5 line chart
PLOT 6 line chart with total line
##Resources - list any sources you consulted to create your visualization

1) This data is from Center For Responsive Ploitics (OpenSecrets.org) and is for non-commercial use only.
2) http://dimplejs.org/index.html

