# NYC CitiBike Sharing Challenge

## Purpose:

#### What do we want to know?
The purpose of this challenge was to determine for investors and potential stakeholders that a bike sharing program in Des Moines, Iowa is a workable business proposal

#### What will we be looking at?
CitiBike has a bike share program in NYC and their data is publicly available. This is a great resource that we will take advantage of. We will take a subset of data and analyze it to try and determine patterns and elements that may translate from an NYC program to a similar one in Des Moines. We will be loking at bike share data from August 2019 as it was a nice summer time when folks were out bike rental was likely

We gathered our data from a publicly accessible source at the following link: "https://s3.amazonaws.com/tripdata/index.html"

Further details can be found here: "https://ride.citibikenyc.com/system-data"

## Results:

I started by using Pandas to turn the trip duration for each ride in the initial data from seconds (integer) to datetime. 

This was the process I used:

<img src="https://github.com/mpournaras/bikesharing/blob/main/Resources/dtCode.png" width="450" height="300">

Once this was complete, we exported to a fresh CSV to begin the graphical analysis in Tableau.

#### How long were the bikes being used for each ride? Did rider gender have any effect?

<img src="https://github.com/mpournaras/bikesharing/blob/main/Resources/Story1.png" width="550" height="500">

It would appear with this data that the vast majority of rides are 20 minutes or less. The peak being right around 5 minutes.

How about the gender break down of the same ride time data? The data for august was broken down as follows:

-**Male**: 65.3%   -**Female**: 25.1%   -**Unknown**: 9.6%

<img src="https://github.com/mpournaras/bikesharing/blob/main/Resources/Story2.png" width="550" height="500">

While males make up the majority of rides, it would appear that ride time per rental is roughly the same and follows a similar distribution.

#### When are users renting the bikes?

We can see from the following figure that the most popular times to rent bikes were **8AM**, **5PM**, and **6PM**. 

<img src="https://github.com/mpournaras/bikesharing/blob/main/Resources/Story3.png" width="550" height="400">

Does this pattern changes when we look at ride times segmented by weekday? Let's have a look!

<img src="https://github.com/mpournaras/bikesharing/blob/main/Resources/Story4.png" width="550" height="400">

We can confirm that during the weekdays (Monday-Friday) the ridership pattern remains. However we see a far more even distribution during the weekends during leisure hours. These are foucused from **11AM** all the way to **5PM**

How about the same data further segmented by gender?

<img src="https://github.com/mpournaras/bikesharing/blob/main/Resources/Story5.png" width="550" height="400">

While we can once again confirm that males make up a vast majority of rider data, the riding time pattern is roughly the same. Focused around business week hours and weekend leisure hours.

#### How are riders paying for and enjoying the rental bikes?

Can the data show us how people pay for these rides? It sure can! The data includes if each rider was a subscriber or a one-time single paying user. We made a graph to display this and stratified it by gender. Let's take a look!

<img src="https://github.com/mpournaras/bikesharing/blob/main/Resources/Story6.png" width="550" height="350">

The **subscribers** wildly out number single **customers** regardless of gender.

#### Where are people starting their rides? Where are they picking up the bikes?

I was able to make a map that showed the starting station that customers used. The stations coordinates were provided which made making a map extremely easy. Is the data helpful? Let's have a look!

<img src="https://github.com/mpournaras/bikesharing/blob/main/Resources/Story7.png" width="550" height="550">

We can see that the bikes are rented heavily in the tourist areas and the financial districts of Manhattan, NY.

## Summary

#### What can we take away from all of this?

Will this project succeed in Des Moines? Des Moines does have a relatively vibrant and dense downtown. The population is obviously less than New York but the bike rental model could adjust.

![](http://res.cloudinary.com/simpleview/image/upload/v1520376833/clients/redesign-desmoines/e8c9801f_9d91_482a_8a7b_cfaa7e0342ad_9b6c0c87-3a83-44fb-8e98-adf1d94e8674.jpg)

* The bikes would need to be most available before and after the "typical" business day.
* The bikes would need to be maintained and available on weekends as well.
* An app would be ideal because the majority are **subscribers**. They need an easy way to get bikes.
* Gender plays very little role in the rental data. I think a single size-fits-all bike would suffice
* The majority of rides are short so there would need to be frequent picking up and re-stationing of the bikes.

#### What else could we look at?

* A visualization showing **common bike paths** would be helpful. Where do they go after they are rented. This could help direct overhead resources to collection and maintenance 
* With "User Type" and "Birth Year" we could visualize what the average age, or age range of users are per type and offer deals/discounts or incentives to get those who are not subscribed to subscribe.
