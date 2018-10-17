I have worked on the bids dataset from CloudFrame that someone shared on the meetup group. The dataset details and the problem is defined below.

Predicting Bid Outcomes for Texas DOT Road Construction Projects

The Data

The file titled texas-bids.csv contains a set of public road construction project letting results from the State of Texas Department of Transportation. Most of the fields are self explanatory, but are defined here. Each row corresponds to a single project.

time: estimated number of working days to complete the project.
estimate: estimated dollar amount of the award.
let_date: the date the project was awarded to the lowest feasible bidder.
length: the length of the construction in miles.
winner: the winning bidder.
win_amt: the winning bid amount.
num_bids: the number of bids submitted to the DOT.
compiled_bids: a structured text field of bidder | amount combinations.
bid_spread: the highest bid minus the lowest bid.
county: the county where the work will take place.
month: the numerical month.
Note that some of these fields are okay to include in the modeling as predictors, while others are not. For example, the model should NOT be allowed to consider winner, win_amt, the amounts portion of compiled_bids, or the bid_spread. Fields like num_bids and the bidder portions of compiled_bids are okay for the purpose of this problem.

Problem:

Construct a predictive model of something interesting regarding winning bids.
