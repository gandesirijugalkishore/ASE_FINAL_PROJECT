# ASE_FINAL_PROJECT BY Jugal Kishore Gandhesiri

FILE STRUCTURE:

1. DATASET
2. SOURCE CODE
3. REPORT AND PRESENTATION

[Product Recommendation System Using NLP]

We want to build a hybrid recommendation engine that will not only recommend similar products but also recommend products in other categories, genres or fields to a shopper in order to help them find what they might not have been looking for.

### Introduction
[About the Amazon Customer Reviews Dataset](https://s3.amazonaws.com/amazon-reviews-pds/readme.html)

[The Multilingual (US) Dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)
- The dataset is too big to upload onto github (3.63gb) but can be found under the multilingual reviews portion of the link.  Just copy and paste the line within the link to the url and press enter to download any of the datasets.

### Exploratory Data Analaysis
[Data Analysis] (https://github.com/gandesirijugalkishore/ASE_FINAL_PROJECT/blob/main/APR_analysis.ipynb)

### Recommendation Modules
[Recommender] (https://github.com/gandesirijugalkishore/ASE_FINAL_PROJECT/blob/main/APR_recommender.ipynb)

[Keyword Search]  https://github.com/gandesirijugalkishore/ASE_FINAL_PROJECT/blob/main/APR_recommender_keyword_simple.

We have found that:

- Over 60% of all reviews receive 5 star ratings.
- Most products have between 100 and 1,000 reviews.
- Most customers give between 1 and 10 reviews.
- Out of 11,500+ products, less than 250 have an average rating under 3.0.
- 90% of the Amazon marketplace revolves around books, music, movies and mobile apps.
- The top 3 categories have intangible products (digital).
- The range in the difference of average categorical ratings is 0.84, from 3.84 to 4.68.
- Over time the average annual ratings stay between 4.1 and 4.4.
- The marketplace has grown exponentially since 2011.
- Average product ratings are mostly affected by 5, 4 and 1 star reviews.
- Most reviews occur in January and December, likely because of the holidays.

In this case, we explore 3 different ways to use collaborative based filtering.

1. The first method suggests products that other users like to a specific user based on their rating of a specific product.  Essentially, it finds users that rated a product similar to the specific user and returns the top products the other users liked.

2. The second method predicts what products a user may like based on past rating history and the rating history of other users.  This method is not specific to the rating of one product like the first method.

3. The third method predicts products similar to a specific product by finding the nearest neighbors to that product.  This method is good for users who may want to purchase products as bundles.

We evaluate our methods by:
- Testing the recommendation systems to see what products they return.
- Understanding matrix factorization and how it effects collaborative filtering systems.
- Selecting and tuning various recommendation algorithms to find the best performing algorithm.
- Understanding estimated ratings vs. true ratings.
- Performing precision@k and recall@k tests.
