---
layout: post
title: Codename - Project Luther
---

### Challenge
For the second challenge of the SF Summer 2018 immersive data science program, each of us was tasked with applying newfound skills of
webscraping and linear regression to tackle a question of our choice. Being an avid skiier and in the market for a new pair for this
season after some surprisingly stealthy rocks took out a 2-inch section of edge on my trusty k2 Annex 98s, I decided to build a model
to predict ski prices. 

### Approach
In order to gather data on ski prices (and fulfill the webscraping requirements for the project) I used Selenium and BeautifulSoup to scrape
the entire catalog of skis listed on Backcountry.com. From each product I gathered information on technical specifications listed such as
ski length, widths, weight, turn radius, and core material, in addition to the target variable: price. After some extended wrangling due
to inconsistent listings and some particularly tricky parsing, I ended up with enough data to attempt a model.

### Analysis + Results
Despite applying a wide range of feature engineering techniques, there was no linear regression model that could account for more than
18% of the variance in price under the most advantageous possible conditions for the model. With more rigorous testing practices, all the
models failed to do significantly better than guessing mean price.

### Further Work
It may be the case that there is no way to get information about ski prices from physical features such as the ones examined, but given
more time I would like to attempt a few strategies for getting some results. For one, it may be that non-physical features such as brand
or some kind of 'hype' metric would provide predictive power when incorporated. It may be that backcountry.com alone simply didn't
provide enough data for meaningful predictive power that might otherwise arise to show up, so incorporating other sources may improve
performance. Most likely, the most improvement may come from timing my data collection more effectively. Since the entirety of the data was
collected in the middle of July when the skis have been listed for nearly an entire year and picked over from the previous season, the only
skis left in the data are both by definition undesirable (perhaps due to mis-pricing) and on varying levels of sale. I plan on rescraping
once new skis are released for the current season to see whether these physical features really don't have any contribution to pricing
in the ski marketplace.
