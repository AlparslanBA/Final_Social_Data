---
showFullContent : true
readingTime : false
hideComments : true
---

## Introduction

Wildfire is the term used to describe an uncontrolled fire. If let lose these could potentially have devasting and life threating consequences of people, towns and environment effected by the fire. Besides the fire itself being dangerous it also heavily increases the air pollution[[1]](https://www.epa.gov/air-research/wildland-fire-research-health-effects-research) which could lead to long complications or even death[[2]](https://www.who.int/health-topics/wildfires#tab=tab_1). Burning of green areas also lead to increase of greenhouse grass emission which negativity impacts the climate and global warming[[2]](https://www.who.int/health-topics/wildfires#tab=tab_1).    

The importance of trying to predict and prevent wildfires is enough reason for us to try and investigate this event. By exploring a potential connection between poverty level and wildfires we would be able to see if there is a group of people in a bigger risk to the devastating consequences. This could also be used to argument for investing in fire safety in these areas if a correlation is found. 
A lot of different factors can play a role in why a wildfire is appearing in the US. These could either stem from natural casus or be a byproduct of human activities (either malicious or accidental).  To investigate this a database contains various information of wildfire in the timespan of 1992 – 2015 [[3]](https://www.kaggle.com/datasets/rtatman/188-million-us-wildfires/code) will be used. Several visualizations will be created to get a better understanding of the information.

A data-set provided by OpenIntro [[4]](https://www.openintro.org/data/?data=county_complete) contains socioeconomic information will be used to investigate and answer the question of: **Is there a correlation between human created wildfire and poverty in the US?** 

*<em>The literature list can be found at the bottom of the website. Each marker ([]) will point to the source website. </em>

_______

## Investigating the wildfire data-set

The dataset relating to wildfires, as mentioned in the introduction, contains 188 million rows with various information of wildfires in the US. 

We start of by diving into the dataset by showing some plots to get a better understanding on the distribution and occurrences of wildfires. We have done this by using boxplot and bar plot to better visualize the magnitude and distribution. 

 ![Test]({{< baseurl >}}/real_part1.png?style=centerme)

The figure to the left illustrates the distribution of the causes of wildfire. This shows that debris burning is having the highest number of occurrences compared to the rest. Miscellaneous and missing/undefined is also having a high distribution, which make sense since it is not an easy task to conclude the origin of a wildfire. Arson is also having a high distribution which indicates that many wildfires is started with a malicious intent. 

The righter plot shows the yearly occurrences of wildfires. Here it can be seen that the oldest and earliest years is quite similar compared on the occurrence rate. In the middle there is a higher average of occurrences. This gives an indication of that wildfires is heading down the right direction but there have bane made no progression compared to wildfires in the 90’s. 

Let’s take a deeper look at the “damage” outcome of the different types of wildfire causes! 

 ![Test]({{< baseurl >}}/real_part2.png?style=centerme)

The plot to the left shows that wildfires created by lightning burns a signification higher average amount of acres land. It is almost 3 time more than the closest one. This is not surprising since natural wildfires is both unpredictable but can also hit the right spot to start a big wildfire. It just takes a small ignition in a dry-forest area to create a devasting and uncontrollable wildfire. Power-line being the second highest makes sense since they are typically placed every area including forest and rural. Other human made wildfires, such as campfire and arson, does not burn a huge amount (compared to lightning) acre. This could be that they are started near the city or have fire safety procedures (which you would assume camping sites have), so it will come under control a lot quicker than the rest. 

The right plot shows that wildfires from lightning also lasts the longest on average. This correlates with the amount of burned acres. What seems surprising is that smoking having one of the highest burn times while on average burning so little acres. On average human created wildfire is extin-guished within a day which is a positive side.

Overall, we can see that nature created wildfires is both more damaging and lasts in a significant longer time. This makes sense since you would imagine that these start by random in random lo-cations. Human made wildfire may be easier to locate early since they are close to places that are visited.

Now it is time to look at the trends for each wildfire cause. An interactive boxplot has been creat-ed to dive deeper into the daily occurrences. By selecting a tap the given weekdays occurrences of the selected cause will be shown. 

{{< include-html "test2.html" >}}

___

This shows that most fires start in the weekend (Saturday and Sunday) and closely followed by Monday. There could be many reasons for this to happened but taking an educated guess would be because people have more free time and relaxed. 
Some of the more obvious ones to populate the weekend is Arson, Campfire children and smok-ing. This make sense since people are off from work and children off from school. There may also be alcohol and narcotic used during these times, which don’t help with taking responsible and safe decisions. Other casus such as railroad and equipment use occurs more often during the working day. Now lets take a look at how it is for each month!


{{< include-html "test4.html" >}}

By looking at the monthly occurrence we see that March, April, July and August are the months with the most wildfires.
Some obvious causes occur more often in summertime which includes campfire and fireworks (because of 4th of July) These months are typically hotter and drier, which makes it even easier for a wildfire to start.
The beginning of spring (Marts, April) is booming in many categories such Arson, debris burning and children. Events such as spring break and easter vacation could be the leading reasons for these.


## Getting an overview of wildfires by mapping

Now it is time to dive in some mapping to see where there are more occurrences. We have dividing the casus into 4 categories being nature(lightning), malicious man-made(Arson), man-made(campfire, children, debris burning, equipment use, fireworks, powerline, railroad) and unknown (miscellaneous, missing/undefined).

On these interactive models, you will be seeing the distribution of fires recorded throughout all the years in the whole United States for all the causes of wildfire. The more you zoom in, the more specific data points you will get on the counties. By taking a look at the maps you will discover in which parts of the USA most of the fires are happening. The maps are ordered after these categories: unknown, natural, man-made, and malicious between the years 2010-2015.

### Unknown cluster map

If we take a look at the unknown marker cluster we can see a lot of unknown fires have happened a lot in Los Angeles, Texas, and Washington states. We can't correlate the reason to anything since it is unknown, but a lot of fires have been spotted here.

<iframe src="https://rawcdn.githack.com/AlparslanBA/Final_Social_Data/fbad5233ad454e93acba41176b89e63856dbd515/static/html/unknown_map.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	height="500"
	scrolling="no"
	seamless="seamless"
	frameborder="0">
</iframe>

### Natural cluster map

The next markercluster map has plotted all the natural causes that have been registered in this dataset. Taking a closer inspection of the map, we can see that most of nature caused fires happened in the west part of the USA. This is another part we can't explain since anything can happen in nature.

<iframe src="https://rawcdn.githack.com/AlparslanBA/Final_Social_Data/fbad5233ad454e93acba41176b89e63856dbd515/static/html/nat_real_map.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	height="500"
	scrolling="no"
	seamless="seamless"
	frameborder="0">
</iframe>

### Man-made cluster map

The third plot we have here is about our category of man-made fires.  While exploring the map, we can see that most fires are happening on the southeastern and south coasts of the USA. The fires happening in this map can be tied to multiple reasons, such as campfires, debris burning, and powerlines breaking m.m. Unusually this is happening a lot more frequently in southeastern states compared to overall in the USA.

<iframe src="https://rawcdn.githack.com/AlparslanBA/Final_Social_Data/fbad5233ad454e93acba41176b89e63856dbd515/static/html/manmade_map.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	height="500"
	scrolling="no"
	seamless="seamless"
	frameborder="0">
</iframe>


### Malicious Man-made cluster map

The last plot we have is about the category of malicious/ill-minded causes. By inspecting the map we can see that the southeastern and eastern parts of the USA consist of most of the malicious fires overall. The most committed malicious fire in the USA is arson (according to our dataset), which could be correlated with our second dataset about poverty.

<iframe src="https://rawcdn.githack.com/AlparslanBA/Final_Social_Data/fbad5233ad454e93acba41176b89e63856dbd515/static/html/natueral_map.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	height="500"
	scrolling="no"
	seamless="seamless"
	frameborder="0">
</iframe>



## Investigating poverty dataset

To help in the investigation of predicting wildfire causes in the U.S. we looked into socioeconomics to see if some correlation could be found. We found an interesting dataset originating from the official U.S. department of agriculture which has conducted monitoring of poverty ratings, education among others. This dataset contains records about the aforementioned topics and more in 2010 for each county in the US.
Before attempting to relate poverty to wildfire, let us have a look at the distributions of the relevant socioeconomic data

 ![Test]({{< baseurl >}}/distri.png?style=centerme)

The above histograms show signs of somewhat right-skewed distributions where poverty, income and higher degrees of education seem to follow each other. This comes as no surprise due to their high correlation, as is also why moving forwards we will only focus on the aspect of poverty. The distribution of poverty ratings seems to be centered around 15% with only few counties having higher general levels of poverty.
To get an understanding how poverty ratings are distributed across America we can plot the data onto a map which gives a nice spatial sense of the tendencies.



# Prediction    


![Test]({{< baseurl >}}/08-05-22-09-33-36.png)

    -


# References

1: EPA. Wildland Fire Research: Health Effects Research. https://www.epa.gov/air-research/wildland-fire-research-health-effects-research. Author: EPA. Last updated: april 14, 2022. Last visited : 10/05/2022

2:WHO. Wildfires. https://www.who.int/health-topics/wildfires#tab=tab_1 Author: WHO. Last visited: 10/05/2022

3: Kaggle. 1.88 Million US Wildfires https://www.kaggle.com/datasets/rtatman/188-million-us-wildfires/code Last updated: 2020. Author: RACHAEL TATMAN. Last visited: 10/05/2022

4: OpenIntro. United States Counties: county_complete https://www.openintro.org/data/?data=county_complete Author: OpenIntro. Last visited: 10/05/2022
