# Amazon_Vine_Analysis
*Module 16*


## Overview
With the recent success of learning and using AWS, a new assignment was given to spend time analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. The purpose of the analysis is to determine if there is any bias toward favorable reviews from Vine members.

## Results
###### How many Vine reviews and non-Vine reviews were there?
To ensure that the analysis being done was helpful, we first filtered out items that had less than 20 total votes. The data was narrowed further by retrieving items where the at least 50% of the votes were considerd helpful. Finally, the remaining data was filtered by paid, then unpaid reviews getting us to the point were some simple counts and analysis could be complete.  Total unpaid reviews: *43,745*     Total paid reviews: *969*
![total_unpaid](https://github.com/RachelRautenberg/Amazon_Vine_Analysis/blob/main/Resources/total_unpaid_reviews.PNG) ![total_paid](https://github.com/RachelRautenberg/Amazon_Vine_Analysis/blob/main/Resources/total_paid_reviews.PNG)

##### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
Total unpaid 5-star reviews: *19,233*       Total paid 5-star reviews: *430*
![5star_unpaid](https://github.com/RachelRautenberg/Amazon_Vine_Analysis/blob/main/Resources/5star_unpaid.PNG)                           ![5star_paid](https://github.com/RachelRautenberg/Amazon_Vine_Analysis/blob/main/Resources/5star_paid.PNG)

##### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
Percentage 5-star vs total unpaid:  *43.97%*     Percentage 5-star vs total paid:  *44.38%*
![unpaid_percent](https://github.com/RachelRautenberg/Amazon_Vine_Analysis/blob/main/Resources/unpaid_percent.PNG)                   ![paid_percent](https://github.com/RachelRautenberg/Amazon_Vine_Analysis/blob/main/Resources/paid_percent.PNG)


## Summary
When working with the office products reviews, the data would suggest that there is not a positivity bias for reviews in the Vine program. Several things would suggest this:
   - [x] The total number of reviews coming from the paid program is very small (969) compared to the total of unpaid (43,745).
   - [x] The total number of 5-star reviews is also small.
   - [x] The percentage of 5-star vs total reviews in both programs is very close, suggesting that the reviews are of similar proportion in both paid and unpaid.

The most critical factor in this analysis is the similarity in percentages of 5-star vs total reviews.  One would expect based on the similar percenatages in the two groups, if the incoming data remains stable to this model, an increase in paid reviews volume would not skew positive reviews with such significance as to make the reviews inapplicable.  

Additional analysis that I would recommend, one of which was completed, would be:
<summary>Determine what percentage of total 5-star ratings came out of paid reviews. In this case that percentage is *2.19*; leaving almost a full *98%* of 5-star reviews stemming from unpaid reviewers. </summary>
    ![5star_comp](https://github.com/RachelRautenberg/Amazon_Vine_Analysis/blob/main/Resources/5star_comp.PNG)
*It may also be helpful to run similar analysis on 1-star ratings to understand if there is negative bias. This would better level set the understanding for the stability of reviews derived from the Vine program.
