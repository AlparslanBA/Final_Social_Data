---
showFullContent : true
readingTime : false
hideComments : true
---

## Technical details

This small chapter provides usefull links!

[A click on this takes will take you to the websites github!](https://github.com/AlparslanBA/Final_Social_Data)

[This will take you to the original wildfire database](https://www.kaggle.com/datasets/rtatman/188-million-us-wildfires/code)

[This will take you to the original poverty database](https://www.openintro.org/data/?data=county_complete)

[This will take you to a drive containing the used databases(they are modified) and the notebook](https://drive.google.com/drive/folders/1srLEJzDa4cwPYw0FIF2fQwZRyUT-p54n)


## Introduction

Wildfire is the term used to describe an uncontrolled fire. If let lose these could potentially have devasting and life threating consequences of people, towns and environment effected by the fire. Besides the fire itself being dangerous it also heavily increases the air pollution[[1]](https://www.epa.gov/air-research/wildland-fire-research-health-effects-research) which could lead to long complications or even death[[2]](https://www.who.int/health-topics/wildfires#tab=tab_1). Burning of green areas also lead to increase of greenhouse grass emission which negativity impacts the climate and global warming[[2]](https://www.who.int/health-topics/wildfires#tab=tab_1).    

The importance of trying to predict and prevent wildfires is enough reason for us to try and investigate this event. By exploring a potential connection between poverty level and wildfires we would be able to see if there is a group of people in a bigger risk to the devastating consequences. This could also be used to argument for investing in fire safety in these areas if a correlation is found. 
A lot of different factors can play a role in why a wildfire is appearing in the US. These could either stem from natural casus or be a byproduct of human activities (either malicious or accidental).  To investigate this a database contains various information of wildfire in the timespan of 1992 – 2015 [[3]](https://www.kaggle.com/datasets/rtatman/188-million-us-wildfires/code) will be used. Several visualizations will be created to get a better understanding of the information.

A data-set provided by OpenIntro [[4]](https://www.openintro.org/data/?data=county_complete) contains socioeconomic information will be used to investigate and answer the question of: **Is there a correlation between human created wildfire and poverty in the US?** 

*<em>The literature list can be found at the bottom of the website. Each marker ([]) will point to the source website. </em>

_______

## Investigating the wildfire data-set

The dataset relating to wildfires, as mentioned in the introduction, contains 188 million rows with various information of wildfires in the US. 

We start of by diving into the dataset by showing some plots to get a better understanding on the distribution and occurrences of wildfires. We have done this by using boxplot and bar plot to better visualize the magnitude and distribution. We will focus on data from 2011 to 2015. 

 ![Test]({{< baseurl >}}/real_part1.png?style=centerme)

The figure to the left illustrates the distribution of the causes of wildfire. This shows that Campire, children and fireworks have some of the higest occurrences. Arson is also having a high distribution which indicates that many wildfires is started with a malicious intent. 

The righter plot shows the yearly occurrences of wildfires. Here it can be seen that the oldest and earliest years is quite similar compared on the occurrence rate. In the middle there is a higher average of occurrences. This gives an indication of that wildfires is heading down the right direction but there have bane made no progression compared to wildfires in the 90’s. 

Let’s take a deeper look at the “damage” outcome of the different types of wildfire causes! 

 ![Test]({{< baseurl >}}/real_part2.png?style=centerme)

The plot to the left shows that wildfires created by lightning burns a signification higher average amount of acres land. It is almost 2 time more than the closest one. This is not surprising since natural wildfires is both unpredictable but can also hit the right spot to start a big wildfire. It just takes a small ignition in a dry-forest area to create a devasting and uncontrollable wildfire. Power-line being the second highest makes sense since they are typically placed every area including forest and rural. Other human made wildfires, such as campfire and arson, does not burn a huge amount (compared to lightning) acre. This could be that they are started near the city or have fire safety procedures (which you would assume camping sites have), so it will come under control a lot quicker than the rest. 

The right plot shows that wildfires from lightning also lasts the longest on average. This correlates with the amount of burned acres. What seems surprising is that smoking having one of the highest burn times while on average burning so little acres. On average human created wildfire is extin-guished within a day which is a positive side.

Overall, we can see that nature created wildfires is both more damaging and lasts in a significant longer time. This makes sense since you would imagine that these start by random in random lo-cations. Human made wildfire may be easier to locate early since they are close to places that are visited.

Now it is time to look at the trends for each wildfire cause. An interactive boxplot has been creat-ed to dive deeper into the daily occurrences. By selecting a tap the given weekdays occurrences of the selected cause will be shown. The bar is plottet left for the label and was not intended. 

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

Two of the maps (uknown and natural) have not been used for this website. This is because it makes the load time way too long. Instead we will just explain what we saw from them. The plots can be found in the notebook link. The unknown cluster showed that these fires happened a lot in Los Angeles, Texas, and Washington states. We can't correlate the reason to anything since it is unknown, but a lot of fires have been spotted here.
The natural causes happen mostly in the west part of the US. 

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

The last plot we have is about the category of malicious/ill-minded causes. By inspecting the map we can see that the southeastern and eastern parts of the USA consist of most of the malicious fires overall. 

<iframe src="https://rawcdn.githack.com/AlparslanBA/Final_Social_Data/fbad5233ad454e93acba41176b89e63856dbd515/static/html/natueral_map.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	height="500"
	scrolling="no"
	seamless="seamless"
	frameborder="0">
</iframe>

We can from the maps see that both malicious and nonmalicious man made fires happens more frequently in the southeastern part of US. This indicates that there is something going on with wildfires in this part of the map.  This will be a interested point to remember when we investigate poverty rating in the US. 

## Investigating poverty data-set

To help in the investigation of predicting wildfire causes in the U.S. we looked into socioeconomics to see if some correlation could be found. We found an interesting dataset originating from the official U.S. department of agriculture which has conducted monitoring of poverty ratings, education among others. This dataset contains records about the aforementioned topics and more in 2010 for each county in the US.
Before attempting to relate poverty to wildfire, let us have a look at the distributions of the relevant socioeconomic data

 ![Test]({{< baseurl >}}/distri.png?style=centerme)

The above histograms show signs of somewhat right-skewed distributions where poverty, income and higher degrees of education seem to follow each other. This comes as no surprise due to their high correlation, as is also why moving forwards we will only focus on the aspect of poverty. The distribution of poverty ratings seems to be centered around 15% with only few counties having higher general levels of poverty.
To get an understanding how poverty ratings are distributed across America we can plot the data onto a map which gives a nice spatial sense of the tendencies.

### Fire count map
<iframe src="https://rawcdn.githack.com/AlparslanBA/Final_Social_Data/bb12094a9335d1e72d99318f75cf4fd3c895eeda/static/html/chok_2.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	height="500"
	scrolling="no"
	seamless="seamless"
	frameborder="0">
</iframe>

### Poverty count map
<iframe src="https://rawcdn.githack.com/AlparslanBA/Final_Social_Data/bb12094a9335d1e72d99318f75cf4fd3c895eeda/static/html/chok_1.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	height="500"
	scrolling="no"
	seamless="seamless"
	frameborder="0">
</iframe>

At first glance one might notice that the southeastern states seem to reside in higher levels of poverty in contrast to the northwestern states. By splitting the data up into four coastal areas, this trend becomes more apparent.

![Test]({{< baseurl >}}/pov_coast.png?style=centerme)

From the figure above we see the tendency for southeastern states to have higher poverty ratings as these coastal regions have nearly 5% higher poverty ratings on average.
An observation which does seem to go in hand with the number of wildfires which also have a tendency to center around the southeastern states.
To get a better overview of how poverty correlates to the number of wildfires in each state for that given year let us have a look at the distributions:

![Test]({{< baseurl >}}/simu_1.png?style=centerme)

![Test]({{< baseurl >}}/sim2.png?style=centerme)

When compared, the immediate correlation seems to somewhat vanish as wildfires appear to be more skewed due to few states having a greater impact. Though it is not as clear, states with higher levels of wildfires seem to be somewhat centered around higher levels of poverty.


## Prediction the cause of wildfire

So far, we have explored aspects of wildfires in America as a means of visualizations. Figures and plots that have helped highlight some of the underlying features and tendencies, which at first glance may be hidden to the naked eye. But to see things more clearly, we need to put on some strong glasses, called machine learning. 
Combining the knowledge we have gained so far with such glasses, we will try to predict what plays a role in wildfires in addition to the influence of education and socioeconomic status in human started fires.
To spare you for the details of machine learning models we will instead refer to our notebook where hopefully your inner nerd can be pleased.  We will instead look at how, with the use of a Random Forest Classifier, we have been able to test and determine the importance of different features that could have an effect on wildfires.
We found that running the model on the vanilla dataset was too little help as it contained way too many redundant features. Features like "SOURCESYSTEMTYPE", which is the type of database the record was drawn from. Not for much use in our case. We therefore manually reduced the dataset to only the most relevant columns and combined it with the socioeconomic dataset.
Running the Random Forest Classifier on this dataset having it classify the cause of fire resulted in a fairly accurate model reaching accuracies upwards of 70%. We noticed how the model made use of features and how some were more prominent than others. To combat this and potentially improve the quality of classification we removed and grouped some of the features e.g., states. With this tweaking the model reached accuracies in the start/mid 70'ies and resulted in the following findings. The figure below displays the magnitude of impact each feature has on the prediction of the wildfire cause.


![Test]({{< baseurl >}}/ml.png?style=centerme)

The immediate front runners are longitude and latitude which would not come as a surprise. The reason for these features to have such a great impact is likely due to their geographical association. With a specific location a lot of implicit geoinformation is conveyed i.e., in the sense of weather, humidity etc for a given area. 
This does raise some attention to the effects of months. As mentioned earlier, one would not be entirely wrong to assume some correlation between months, along with the seasonal change, and wildfires. However, this does not seem to be the case as the influence of month only contributes by a small fraction. Furthermore, we see that the magnitude of weekdays is like that of months, which would indicate that our model is influenced greater by location than time.         
What is worth noticing is the magnitude of which the poverty rating of counties seems to influence wildfires in America. This does seem to play apart with the previously mentioned about a possible relationship between the southern states, their relative poverty rating and the number of wildfires.

## Discussion

In the first part of the research we jumped in and investigated the wildfire dataset. This showed us that Arson, campfire, children and firework are the most frequent reasons for wildfire. By comparing man made fires with nature we saw that nature fires burns the most acres and lasts the longest. This could be, as mention, because they occur in random, dry, forest areas and runs out of control. Most fires seems to occur in the weekend while they also occur the most in summer and spring. By looking at maps we can clearly see that most man-made cases occur near the southeastern side of the US. This indicates that there is need for more fire safety learning, safety investment and preparetion in these areas. 

After conducting an analysis of the socioeconomics dataset we found high correlation between the four initially selected attributes. This made the reasoning for focusing on poverty. Furthermore combing the datasets some correlation could be found with regards to higher levels of poverty and states grouped in the southeastern region(by looking at the maps). This seemed to compliment our investigation question but become less apparent when working with states.

While we can’t say that poverty is directly related to fire, based on our results, it still seems that it plays a role for the origin. By researching others' findings we can see that this research has been done several times. This article [5] discusses how poor areas in Hamilton are more fire proven than the richer. Smoking, overcrowded houses and equipment were some of the main causes. Another article [6] also suggests that there is some influence of poverty when researching fires. A third article[7] also investigates the relation between fire and socioeconomics. Here several socioeconomic factors are investigated.  

## Summary

If you have made it till the end, then cheers!

Our initial research can be used to further investigate the correlation between wildfire and socioeconomic. We have not found a clear indication of a correlation between wildfires and poverty, but there still seems to be some form of a relation. This is confirmed by the different articles mentioned in the discussion part. By looking at the maps we can clearly see that the southeastern area is more at the risk than the rest of the US. Future work could mainly focus on this part of the US to further improve fire safety andprovide help and guidance to prevent further unnecessary wildfires. 

## Bibliography

1: EPA. Wildland Fire Research: Health Effects Research. https://www.epa.gov/air-research/wildland-fire-research-health-effects-research. Author: EPA. Last updated: april 14, 2022. Last visited : 10/05/2022

2:WHO. Wildfires. https://www.who.int/health-topics/wildfires#tab=tab_1 Author: WHO. Last visited: 10/05/2022

3: Kaggle. 1.88 Million US Wildfires https://www.kaggle.com/datasets/rtatman/188-million-us-wildfires/code Last updated: 2020. Author: RACHAEL TATMAN. Last visited: 10/05/2022

4: OpenIntro. United States Counties: county_complete https://www.openintro.org/data/?data=county_complete Author: OpenIntro. Last visited: 10/05/2022

5: The Hamilton Spectator. When fire meets poverty: The economics of fire https://www.thespec.com/news/hamilton-region/2017/04/01/when-fire-meets-poverty-the-economics-of-fire.html Author: Steve Buist and Teviah Moro. Last updated : 03/03/2020. Last visited: 10/05/2022

6:NFPA research . Poverty and the Risk of Fire https://www.nfpa.org/~/media/Files/News%20and%20Research/Fire%20statistics%20and%20reports/US%20Fire%20Problem/ospoverty.pdf Author: Rita Fahy, Ph.D. and Radhika Maheshwari. Last updated : 07/2021. Last visited: 10/05/2022

7: Federal Emergency Management Agency
United States Fire Administration
National Fire Data Center. SOCIOECONOMIC FACTORS AND
THE INCIDENCE OF FIRE https://www.usfa.fema.gov/downloads/pdf/statistics/socio.pdf Author: Federal Emergency Management Agency
United States Fire Administration
National Fire Data Center. Last updated : 06/1997 Last visited: 10/05/2022
