# NYC CitiBike Sharing Challenge

## Purpose:

#### What do we want to know?
The purpose of this challenge was to determine for investors and potential stakeholders that a bike sharing program in Des Moines, Iowa is a workable business proposal

#### What will we be looking at?
CitiBike has a bike share program in NYC and their data is publicly available. This is a great resource that we will take advantage of. We will take a subset of data and analyze it to try and determine patterns and elements that may translate from an NYC program to a similar one in Des Moines. We will be loking at bike share data from August 2019 as it was a nice summer time when folks were out bike rental was likely

We gathered our data from a publicly accesible source at the following link: "https://s3.amazonaws.com/tripdata/index.html"

Further details can be found here: "https://ride.citibikenyc.com/system-data"

## Results:

I started by using Pandas to turn the trip duration for each ride in the initial data from seconds (integer) to datetime. 

This was the process I used:
![file]()

Once this was complete we exported to a fresh CSV to begin the grpahical analysis in Tableu.
