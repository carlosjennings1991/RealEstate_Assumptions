# Real Estate Assumptions

Challenging your assumptions about the Real Estate market, specifically who is selling and who is not.

___

For my final project at George Washington University, I designed a machine learning model that predicted whether or not a home would sell in Los Angeles a four year period. 

As a part of my previous job, I had access to neighborhood data which we call 'farms' in the industry. These data sheets contain information like owner names, property info, but most importantly - <b>financial information</b>.

- [x] Assessed Value
- [x] Tax Amount
- [x] Date of Purchase
- [x] Loan Amount

Now, Los Angeles is a big place, so this study focused on the 7 key neighborhood, as shown below. 

<img src="https://github.com/carlosjennings1991/RealEstate_Assumptions/blob/main/Neighborhood_Map_2.png">

___

The mechanics of the machine learning model can be found here - https://github.com/mhorstman/Final_Project_Team_1, the purpose of this repo is to showcase the very suprising finding about <i>who</i> is selling. 

### Assumption 1: Those who have lived in their homes the longest are more likely to sell

<i> i.e the downsizing Baby Boomer </i>

<img src="https://github.com/carlosjennings1991/RealEstate_Assumptions/blob/main/baby%20boomers.jpeg">

Since 2011, <b>2 Million Baby Boomers</b> have retired per year. Are they the largest segment of sellers?

##

### Assumption 2: Those with the most equity are more likely to sell. 

<i> i.e cashing out, plain and simple </i>

<img src="https://github.com/carlosjennings1991/RealEstate_Assumptions/blob/main/piles%20of%20cash.jpeg" width="720" height="480">

Are sky-high valuations prompting owners with tons of equity into selling?

##

### Assumption 3: Those with the lowest, or absent, loan burdens are most likely to sell.

<i> i.e nothing keeping them there </i>

<img src="https://github.com/carlosjennings1991/RealEstate_Assumptions/blob/main/paid%20in%20full.jpeg" width="720" height="480">

<b>38 percent</b> or owner-occupied units are owned free and clear. Without a mortgage tieing them to the property, are these people moving?

##

## Results:

It turns out, all of this assumptions are wildly incorrect. Granted, twenty years ago they may have been true with the GI Generation/Silent Generation taking the place of the Boomer generation, but a lot has changed in 20 years, especially in Los Angeles. 

The image below is the breakdown of several key stats in each neighborhood, comparing sellers vs non-sellers. 

<img src="https://github.com/carlosjennings1991/RealEstate_Assumptions/blob/main/neighborhood_stats.png">

From the above we can see several things. 


- [x] Sellers are more likely to be absentee owners AND live out of state.

- [x] Sellers have more expensive homes compared to non-sellers.

- [x] Sellers have newer homes compared to non-sellers.

- [x] Sellers bought their home at a higher price vs non-sellers.

- [x] Sellers bought their homes more recently vs non-sellers.

- [x] Sellers pay more in property taxes vs non-sellers.

- [x] Sellers have a higher existing mortgage burden vs non-sellers.

##

While the discrepencies in mean values do tell a story, what is much more interesting is the <i>distribution</i> of those values. The mean values simple show what the 50th percentile looks like for sellers and non-sellers in each neighborhood for each statistic we care about.

However, when we look to the left and right of the mean for each metric, we begin to more fully understand the difference between sellers and non-sellers.  

<br>

### Property Taxes: Sellers vs. Non-Sellers
##
<img src="https://github.com/carlosjennings1991/RealEstate_Assumptions/blob/main/Tax_Amount_SFRs.png">
