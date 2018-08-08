In progress

# Predicting Bid Outcomes for Texas DOT Road Construction Projects
Do your best with the attached data and problem as it's described here, and let us know how you did <work@cloudframe.io>.

<https://xkcd.com/356/>

## The Data
The file titled `texas-bids.csv` contains a set of public road construction project letting results from the State of Texas Department of Transportation.  Most of the fields are self explanatory, but are defined here.  Each row corresponds to a single project.  We may update this repository with newer data from time to time.
* `time`: estimated number of working days to complete the project.
* `estimate`: estimated dollar amount of the award.
* `let_date`: the date the project was awarded to the lowest feasible bidder.
* `length`: the length of the construction in miles.
* `winner`: the winning bidder.
* `win_amt`: the winning bid amount.
* `num_bids`: the number of bids submitted to the DOT.
* `compiled_bids`: a structured text field of `bidder | amount` combinations.
* `bid_spread`: the highest bid minus the lowest bid.
* `county`: the county where the work will take place.
* `month`: the numerical month.

Note that some of these fields are okay to include in the modeling as predictors, while others are not.  For example, the model should NOT be allowed to consider `winner`, `win_amt`, the amounts portion of `compiled_bids`, or the `bid_spread`.  Fields like `num_bids` and the bidder portions of `compiled_bids` are okay for the purpose of this problem.  

## The Task
Construct a predictive model of __something interesting__ regarding winning bids.  That something is up to you.  Good models will be constructed using best practices and defensible under rigorous scrutiny.  

## The Submission
Send a description of what you did and model metrics that show how the model performs to <work@cloudframe.io>.  We'll be in touch regarding next steps after we've had a chance to review what you sent.  In particular, we'll judge initial submissions by:
* Is the model constructed to predict or forecast something interesting?
* Is the technique chosen appropriate?
* Are the metrics reported realistic and reasonably performant?

Do NOT send code or model objects.

## The Next Steps
If you're willing and your submission warrants, we'll ask for a follow-on interview.  During that conversation we'll be figuring out if there's a mutual fit between your career aspirations and CloudFrame's opportunities for Data Scientists.  Relevant to this submission, we'll ask you to walk through, in code, how you tuned the chosen algorithm and trained the best model.  We'll want you to describe the entire process verbally, including:
* Data munging.
* Data visualization and exploration.
* Feature engineering.
* Algorithm selection.
* Hyperparameter tuning.
* Testing and validation.

Successful candidates will be able to explain what they did, why, and where their analysis is lacking.  If there's a mutual fit, we'll schedule an in-person interview at a time and date that works for us and you.  

If you have questions, please send them to <work@cloudframe.io>.  We look forward to hearing from you!
