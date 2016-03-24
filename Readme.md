Task 1: Number of helpful votes of a review

Modelled the ratio nHelpful/outOf using regression.

Features that worked.
1. Number of words in reviewText
2. Number of words in the summary
3. Rating given in that review
4. Number of reviews that the user has written with non-zero outOf votes
5. Number of review that the item has
6. Number of punctuations in reviewText
7. Number of punctuations in the summary
8. Number of capital letters in reviewText
9. Number of capital letters in the summary
10. Number of outOf votes the review has.
11. Sentiment analysis score – a review is helpful if the rating is high and the review is highly positive or the rating is low and the review is highly negative
12. Step function for rating
13. Automated readability index (ARI)
14. Rating deviation from mean

Features that did not work.
1. Age of the review
2. Average rating of the item
3. Average rating given by user to any item
4. Using step function for reviewText length

Task 2: Rating Prediction

I implemented a latent factor model for predicting the rating of the books. We are treating user and item features independently. This is most probably because we did not have enough data for user-item feature modelling, that is, a user had rated only a few books. So we were not able to fit a good model to this data.
