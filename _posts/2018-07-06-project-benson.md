---
layout: post
title: Metis Project 1 -- NYC Subway Data EDA
---

### Challenge
For the culminating project of week one for the Metis SF Summer 2018 Data Science cohort, the unstoppable 3-man data science machine consisting of classmates AJ Davis, Pablo Nieto Ramos, and myself were commissioned by the completely fictional yet nonetheless estimable organization Women Tech Women Yes to help promote their upcoming annual summer gala. Their declared strategy was to send volunteers to canvas MTA subway stations in their home city of New York, signing up passersby to attend the free gala and ideally donate to the cause.

### Strategy
In order help WTWY deploy their volunteer resources to maximum effect, we sought to offer concrete recommendations of


**WHERE** - what stations to go to

**WHEN** - at what time of day, and

**WHY** - on what day of the week. Hang on a minu..**MOVING ON**


So, we tasked ourselves with identifying foot traffic patterns for MTA stations.


But being the unstoppable 3-man data science machine that we are, we didn't stop there. No -- for Women Tech Women Yes sought exposure not just to any old commuter passing by on their way in or out of the subway, but rather the kind and powerful souls who would take an interest in their cause, attend their gala, and preferably fork over some of their hard-earned capital reserves for the advancement of the species. 


Thus, 2 orders of business:
1. Determine which stations at which times have the most people passing through
2. Establish the target demographic and where they might be more likely to be.

Starting with 

### Order of Business No. 2
Because.

After considering the specifics of cause and consulting the [literature](https://repository.upenn.edu/wharton_research_scholars/126/), we wanted to pursue those commuters who fit the profile of the with high-income female tech professional. As proxies for each of these attributes we drew data from [Zillow](https://www.zillow.com/new-york-ny/) on housing-prices to account for income, a [Department of Youth and Community Development survey](https://data.cityofnewyork.us/City-Government/Demographic-Statistics-By-Zip-Code/kku6-nxdu) which included gender information by zip code, and The [2016 NYC Tech Ecosystem Report](http://abny.org/images/downloads/2016_nyc_tech_ecosystem_10.17.2017_final_.pdf) on tech density in the city.


![Tech Clusters]({{ site.url }}/public/tech_density_nyc.png "Whatever, San Francisco still has more")


Then, our target demographic well-targeted, we naturally proceeded to

### Order of Business No. 1
Knowing where all the well-payed tech industry women are more likely to be around is all well in good, but ultimately this compaign is about getting the _word_ out to the **PEOPLE**. So where + when are the most of said people passing through NYC subway stations? Luckily, the MTA (for some reason) keeps public weekly logs of turnstyle counters for every turnstile in every station, which we were happy to raid for information on the three weeks leading up to the gala for the past 3 years. Less luckily, there's some funky stuff going on with those numbers, but again luckily here we were a crack 3 man team of _DATA SCIENTISTS_ ready to get all _SCIENCE_ up on some _DATA_, which we totally did. 


![Foot_Traffic]({{ site.url }}/public/all_station_foot_traffic.png "It was basically just like that one scene in The Matrix Reloaded starring Pablo as Neo and DATA as all those Agent Smiths")


Breaking the data into morning and afternoon chunks for each day of the week allowed us to identify individual shifts for WTWY volunteers and rank them by how many people a volunteer at a given station for a given time would expect to see. Which led us to our

### Analysis
Though swimming in pools of relevant information, we still needed to come up with an actual recommendation to provide for the luminaries at WTWY and prove our worth. So we implemented an INCREDIBLY COMPLEX (not really) and TOTALLY ARBITRARY (yes really) weighted algorithm to score shifts based on our vast hoard of data.


![Behold! The DECIDINATOR]({{ site.url }}/public/Weird-machine.jpg 'Don't even think about asking it where you two should go out to dinner, it is so tired of _always_ being the one who has to decide where you go out to dinner!')


With all these powers combined, we were able to provide 

### Results
![recommendation table]({{ site.url }}/public/table.png 'TOP 10 ABSOLUTE BEST MTA STATIONS TO PROMOTE WTWY! YOU WON'T BELIEVE NUMBER 7')
Above are listed the 10 shifts Women Tech Women Yes should **ABSOLUTELY** cover with volunteers in the weeks leading up to the gala. Want to see more? For the low low monthly subscription fee of $199.99, WTWY can access ALL the recommendations and ALL the expertise of renowned 3-man data science machine Davis, Nieto Ramos, and Broer, Attorney's at Law. Activate your account today and receive all the following empty promises at NO EXTRA CHARGE!
* Further refinement of data cleaning techniques and additional data sources for ENHANCED RECOMMENDATION POWER
* Remember that arbitrary decision function? We want YOUR input to tailor it to YOUR needs!
* Ever use a web portal? Of course you have! Aren't they fun? We'll make one for you! For all your future gala needs!
* If you're lucky, Pablo will whistle you a jaunty tune, AJ will gift you mustache hair of incommensurate value, and Sam will take credit for work he didn't do! Definitely just kidding about that last part though.

### Conclusion
Women Tech Women Yes has a vision. It is a vision that encapsulates some of the greatest qualities of our great nation: Liberty, Equality, Ingenuity. Take the sturdy wings of this great vision, and soar on the buffeting winds of change and passion! With the help of our Data Science Compass(tm) services, you can chase down and capture that horizon, feel it wriggle in your bare hands, and bask in the glory of your victory.

Thank you for reading.
