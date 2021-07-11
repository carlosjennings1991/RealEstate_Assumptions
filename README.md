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

The density distribution graph above shows the spread of tax amount for both distributions i.e sellers and non-sellers. What we see here is that non-sellers are vastly overrepresented on the left half of the distribution, and sellers are overrepresented on the right half of the distribution. 

What does this mean? It means that there are a lot of non-sellers paying much, much less than the mean tax amount. 

<br>

### Assessed Total: Sellers vs Non-Sellers
##
<img src="https://github.com/carlosjennings1991/RealEstate_Assumptions/blob/main/Assessed_Total.png">

With a small exception at the left edge of the distributions, non-sellers exceed sellers by a wide margin to the left of the mean. This means non-sellers own homes that have lower assessed values. 

<br>

### Previous Purchase Price: Sellers vs Non-Sellers
##
<img src="https://github.com/carlosjennings1991/RealEstate_Assumptions/blob/main/Previous_Purchase_Price.png">

The above chart shows the sharpest distinction of all the metrics. While the difference in mean previous purchase price is substantial, about $370k, a significant chunk of non-sellers paid <b>far below</b> the mean purchase price. 

There is an interesting California-specific reason for this - Prop 13. 

Prop 13, which passed in the 1970's, basically freezes the property taxes an owner pays to the rate they paid when they purchased the property. So if you bought your home in 1977, your property taxes have barely increased, <i>despite</i> massive increases in property values. Secondly, you can gift the property to your children and <i>they</i> would pay the same amount in property taxes as when you initially bought the property. 

An unforseen side-effect of Prop-13 has been that homes which pay an extraordinarily low amount in property taxes have become a prized family heirloom. Because of this many homes which otherwise would have entered the sales market, are kept out of it, or at the most become rental properties. 

<br>

### Loan Amount: Sellers vs Non-Sellers
##
<img src="https://github.com/carlosjennings1991/RealEstate_Assumptions/blob/main/Loan_Amount.png">

First of all, the above graphic shows the initial loan amount, so even if you now own your home outright, but had an initial loan of $300k, you'd still show up on the chart in the $300k column. However, if you paid your home in cash and never had a loan to begin with, you do not show up on the graph. 

At any rate, we can see non-sellers are clustered to the left side of the chart and sellers towards the right. This tells us that sellers have a higher initial loan amount compared to non-sellers.

<br>

### Year of Purchase: Sellers vs Non-Sellers
##
<img src="https://github.com/carlosjennings1991/RealEstate_Assumptions/blob/main/Year_of_Purchase.png">

The above graphic is my personal favorite because it tells so many stories. First of all, it explains some of the previous charts. 

<b>Q1: Why are sellers paying more in property taxes?</b> Because they purchased more recently. 

<b>Q2: Why are sellers paying a higher mortgage?</b> Because they purchased more recently, and therefore at a higher purchase price. 

It also shows us some recent economic history. Home values increased dramatically in Los Angeles between 2010 and 2020. So even if you purchased in 2016, and sold in 2021, you'd still be making money even after closing costs. Furthermore, if you were afraid that home values would decline over the next 5 years, and are currently paying a very high mortgage, you would want to sell now - and the chart shows that. Secondly, you would not have lived in the area that long and may not be as emotionally tied to a neighborhood. Consequently, a disproportionately high percentage of sellers purchased within the past 10 years. 
