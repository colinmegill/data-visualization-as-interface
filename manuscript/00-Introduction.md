# Introduction

### Prelude by example

Data visualization are becoming a richly interactive interfaces. Studying how to get this right, by way of critical case studies, is the topic of this book. For example, go take a look at [Redfin](http://redfin.com). It is:

- a stand-alone web application
- backed by live data
- capable of moving fluidly between single items, and (by clustering) the entire dataset - see: ![redfin map zoomed out](/images/redfin-zoomed-out.jpg)
- sortable, filterable, searchable, clickable, hoverable, zoomable
- consuming third party API's (namely Google Maps)
- the basis of an entire company
- worlds away from static graphics in process and utility

To further stake out the territory, let's examine [Crossfilter](http://square.github.io/crossfilter/) by Square. In what way can we say this is a similar domain? The controls are different, the output is different. But there is a principle apparent: we begin by showing all of the data - in this case a list of flights rather than a map of houses - and we have powerful filters at our disposal to tell the story _we_ are most interested in, which may be one of trillions or more possibilities. This is what makes interactive data visualizations so amenable to consumer experiences (just as [Zappos](zappos.com) allows me to tell the 'Size 9.5 Men's Crosstrainers in Black under $150' story).

Finally, consider [Crimespotting](http://sanfrancisco.crimespotting.org/#dtstart=2010-04-21T20:35:28-07:00&lon=-122.470&zoom=12&lat=37.778&dtend=2010-04-28T20:35:28-07:00&hours=0-23&types=AA,Mu,Ro,SA,DP,Na,Al,Pr,Th,VT,Va,Bu,Ar). Though it came out a few years after [GapMinder](http://gapminder.org), it was the first interactive data visualization I'd seen (***generalize) that mixed different kinds of controls together

###

Though The first example I saw, built in flash, Hans Rosling's Gapminder was inspirational, but changing the x and y axis wasn't enough to explode my mind into the infinitely combinable 

Before the browser, there was little opportunity to allow drilling, sorting, filtering, dynamic coloring, clicking, hovering, transforming. Different states or configurations meant duplicating the visualization itself, since it was static. In a magazine, we show only what we mean and exactly what we mean to show: it can never change. If we want to show additional views into the data, we repeat the chart.

In the browser, we can interact with the data visualization, and it opens up a new possibility that we’ll explore for the rest of the book: we can show all of the data in one place. Viewers become users, and are no longer passive - they can explore and find their own stories in the data.

It also frees us up to tell as many stories as we want. Adding several buttons that immediately subset the visualization to a particular state, for instance, not only allows us to quickly compare states, but highlights the control the user will later use to explore.

[parallel coordinates nutrition]

Parallel coordinates demonstrate this neatly. What can we see without doing anything? Well, for one, there’s much higher variation in how much water and carbohydrates foods contain than vitamin C, sodium or, to a lesser degree, fiber. When we interact, we subset a list below that highlights certain foods. The highest calorie foods are fats. Cereals are high carb. These are statements of similar character across several dimensions, in plain English, derived from simple actions and interpretation. 

The visualization has 14 brush controls that subset a list below, and in this way, the entire visualization itself is a control for the list. The list, in turn, could include hover, click, sparklines, etc. This flexibility yields extraordinary expressivity.

Similarly, we can tell many stories about cars built in the 70’s and early 80’s: heavier cars have lower efficiency. Cars got lighter over this time period, and they got more efficient. The highest fuel efficient cars are also the lightest. That may have been what the author wanted us to find, or it may not have. I was intrigued by fuel efficiency, but since I have environmentalist leanings, that’s a bias I bring to the visualization. A gearhead might point to the 8-cylinder cars built in 1970 and drool, bemoaning that none were built after 1973.

[parallel coordinates ]

Another advantage: we can see patterns that emerge in aggregate. It looks like on average, cars take about 16 seconds to accelerate to 60mph.



These data sets are not live, they are static. Entirely new worlds emerge when we hook the visualization up to live data sets.

Similarly in principle, but vastly different in practice, is the Redfin web application. 



The visualization, which is the core of the application experience, has every house in their system on one map. It has no opinion on where I live - that is abstracted into a control - or how much money I have to spend - that is too. Pity the poor real-estate catalog printers who distribute custom reports of available houses to people’s mailboxes. Pity the consumer of the information, where the information must be repeated over and over again, and irrelevant information is never removed to lessen the amount one must scan. And finally pity the trees.



This book attempts to remain implementation agnostic, but we love the browser and that may bleed through.

The 
