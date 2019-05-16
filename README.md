# US MASS SHOOTINGS ANALYSIS

## Dataset
platform:https://www.kaggle.com/zusmani/us-mass-shootings-last-50-years

## Introduction
This dataset records 398 mass shootings happened in the U.S that have caused 1996 deaths and 2488 injured in last 50 years. In my country, China, the gun was banned and I wonder, in America, where guns are allowed to be purchased, how shootings distribute across the country and would like to explore the reasons behind these attacks. To be more specific, the questions I am curious about would be like:
- What cities and states are prone to such attacks?
- How many shooters have some kind of mental health problem? 
- Is there any correlation with calendar dates?
- Any correlation with between shooters and their genders and races?

## Summary of data

*Totally, 323 shootings and 21 features*

- Title - Description about the shooting
- Location - location of the mass shooting
- Date - date of shooting
- Incident Area - Area where shooting occurred
- Open/Close Location - Whether the location is closed or opened
- Target - Is it a targeted shooting or random one? If so, who was targeted
- Cause - cause for the shooting
- Summary - brief summary of the shooting. Who shot and the background etc.
- Fatalities - how many were dead during/after the shooting
- Injured - how many were injured during/after the shooting
- Total victims - total victims impacted during the shooting
- Policeman Killed - Number of policeman killed
- Age - Age of the gunman committing the crime
- Employeed (Y/N) - Was the gunman employed
- Employed at - If employed, employment details of the gunman
- Mental Health Issues - Was the gunman mentally ill?
- Race - race of the gunman
- Gender - race of the gunman
- Latitude - locations latitude
- Longitude - locations longitude

## Exploratory Data Analysis

### Trends in 50 years
<img width="1251" alt="scatter" src="https://user-images.githubusercontent.com/40588854/57881042-2d1b1600-77d5-11e9-8a6b-46bfefb72a68.png">

Total Victims, fatalities, injured are showing increasing trends, the count of mass shootings also increased in the past but dropped down in 2017. It makes sense to some extent, because technologies are becoming advanced and some of them are even more easier to accessed by criminals. But it’s not totally reliable as some of them were not recorded for some reasons.

### Race and Victims
<p align="center">
<img width="831" alt="histogram" src="https://user-images.githubusercontent.com/40588854/57881043-2d1b1600-77d5-11e9-99a8-54aa36a90038.png">
</p>

Among the shooters, most of them are white and black. Let’s take a close look to the relationship between race and total number of victims in the following treemap.
<p align="center">
<img width="630" alt="treemap" src="https://user-images.githubusercontent.com/40588854/57881044-2d1b1600-77d5-11e9-8004-f2f0c42dfc63.png">
</p>
From the Tree-map below, white accounts for roughly 60%, at least 3 times larger than black. But, this statistic doesn’t not give any clear picture as USA has predominantly more white people, followed by black and then other minorities like latinos, Asians, native Indians etc. The details aren’t clear enough to draw any inference based on the race of the shooter.

### Cause behind Mass Shootings
<p align="center">
<img width="1042" alt="piechart" src="https://user-images.githubusercontent.com/40588854/57881046-2db3ac80-77d5-11e9-952e-40c394e4136d.png">
</p>

Most mass shootings are caused by psycho and terrorism whose sum can be more than 50% in the cause proportion. Now we have explored some variables such as total victims, Race, and cause behind that, it would be more interesting if we introduce one more variable: Mental Heath Issues and put those things together.

### Relationship among total victims, cause, and mental health issues
<p align="center">
<img width="1288" alt="interactive" src="https://user-images.githubusercontent.com/40588854/57881047-2db3ac80-77d5-11e9-85a8-0815e6c7136e.png">
</p>

It’s worth noting that there are still certain number of shooters with no mental health issues, and some of them are psycho, though. Another point is that nearly all Asian American are terrorists with mental issues.  But still, unknown mental health state takes up a majority of them. There are many people with mental health issues due to abusive childhood, bullies, poisonous environment, job opportunities etc. Medicine cannot solve this issue. Main factor to solve this problem is to have great community of people around. Thats just too difficult to find. 

### Attacks on Weekdays and Weekends
<p align="center">
<img width="658" alt="barchart" src="https://user-images.githubusercontent.com/40588854/57881048-2db3ac80-77d5-11e9-8a7b-665f7a631e8a.png">
</p>

The number of total victims on weekends was obviously more than that on weekdays. More outliers occur on weekdays as well. Mass Shootings usually occur on public areas which are crowed on weekends.

### Mass Shootings across states in US
<p align="center">
<img width="1028" alt="Chloropleth Map" src="https://user-images.githubusercontent.com/40588854/57881053-2e4c4300-77d5-11e9-88b7-d98e695fccd8.png">
</p>

From the perspective of states, California, the brightest region, is the state where there were most total victims in mass shootings. Texas also suffered from mass shooting with lots of casualties. However, some states like North Dakota in which there are no records of mass shooting therefore no victims as well.

### Locations and Fatalities
<p align="center">
<img width="735" alt="Bubble Map" src="https://user-images.githubusercontent.com/40588854/57881049-2db3ac80-77d5-11e9-83ed-40e7dd63d3ff.png">

Points are obviously denser in the east than that in the west. The biggest bubble in the plot indicates the large-scale shootings happened in Las Vegas, and more than 26 people were killed during the event.

### Calendar Heap Map of total Victims in recent 4 years
<p align="center">
<img width="775" alt="HeatMap" src="https://user-images.githubusercontent.com/40588854/57881050-2db3ac80-77d5-11e9-9155-2b7a39839cf7.png">
</p>

We can grab a few points from this heat map:

1. In 2015, mass shootings distribute evenly across the whole year. 
2. However, in 2016, Mass shootings was concentrated from Jan to May.  
3. The total number of victims declined sharply in 2017.
4. Most grids in deep red are lying on Sunday and Saturday.

## Storyline

All exploratory data analysis above are summaries of mass shootings happened in US. But what if I zoom in a certain area, such as the mass shootings in Schools, is there any interesting things that I cannot tell from macroscopic view?  To grad a general sense of how the trend of shootings in school along the time, I drew a line plot and a super interesting finding came up. If we notice the gap between the gap between peaks, we would find that the large-scale shootings in schools took place in a period of around 10 years (1976, 1988, 1998, 2007). The reason of that is really hard to tell but at least we can deduce that the shooters are getting more access to buy lethal weapons, as those peak values were were getting higher along the time. 
<p align="center">
<img width="1259" alt="Stacked area" src="https://user-images.githubusercontent.com/40588854/57881052-2e4c4300-77d5-11e9-885e-328586801cba.png">
</p>

Since the data in 2007 is significantly different from others, I can’t help searching more details about that. The massacre, called Virginia Tech shooting, occurred on April 16, 2007 at the Virginia Polytechnic Institute and State University. The murder, Cho, Cho had previously been diagnosed with a severe anxiety disorder. Because he was not institutionalized, he was still allowed to purchase guns. The shooting prompted the state of Virginia to close legal loopholes that had previously allowed individuals adjudicated as mentally unsound to purchase handguns. Apart from that, according to investigation, only 3% of adults own 50% of  guns in the US, which sounds horrible. It seems there is no central repository to have tracking information of guns bought by individuals across the country. To prevent more innocent lives from being taken away, government should take actions without any delay.

## Conclusion

- The number of victims and mass shootings are increasing drastically from 2014, due to the fact that people are getting easier access to buy guns and weapons than before. 
- Many massacre came from mental issues, but in some states,  there are still no limitations of buying guns to those who have mental health problem.  
- Many mental illness comes from people’s experience in their childhood. To help them, it’s necessary to provide them with a real community full of love and hope. They need to be cared.

## Citations
https://public.tableau.com/profile/rujuta.kortikar#!/vizhome/MassShootingsintheUS/Dashboard1
https://charts.qlikcloud.com/59fdb5cbf917260e00ce5f65/chart.html
https://bl.ocks.org/intellipi/raw/bcbe186b0087c799b3dd26773f623eaa/
https://bl.ocks.org/intellipi/raw/eba6ea42d28af2c4c35010e61ab86a7b/
https://www.kaggle.com/sanarasheed/exploratory-analysis-of-mass-shooting-in-usa
https://www.kaggle.com/kanncaa1/why-gun-violance-increase-in-texas
https://www.washingtonpost.com/news/wonk/wp/2016/09/19/just-three-percent-of-adults-own-half-of-americas-guns/?noredirect=on&utm_term=.cc4d42b2216b
https://en.wikipedia.org/wiki/Virginia_Tech_shooting
