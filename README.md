
##Summary -

This data is from Center For Responsive Ploitics and is for non-commercial use only:
https://www.opensecrets.org/outsidespending/index.php?type=A

In this project, I'll be improving the first chart on the above page, titled "Outside Spending by Cycle Thru December 18th of Election Year, Excluding Party Committees." This plot shows the following types of spending over time:

-*Independent Expenditures*: "An independent expenditure, in elections in the United States, is a political campaign communication that expressly advocates for the election or defeat of a clearly identified candidate that is not made in cooperation, consultation or concert with or at the request or suggestion of a candidate, candidate’s authorized committee or political party."
-*Communication Costs*: communication costs are internal political messages generally aimed only at the members of a union or organization, or company executives. These may be coordinated with the candidates and can be paid for directly from the organization's treasury.
Electioneering Communications: The law applies to "electioneering communications," which are defined as

	broadcast ads (television or radio) airing within 30 days of a primary election or 60 days of a general election that mention or refer to a federal candidate and are aimed at 50,000 or more members of the electorate of the office the candidate is seeking.
*source: Wikipedia, OpenSecrets.org



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



