# Skincare-Recommendation
## Recommending Skincare Products with Natural Language Processing + Deep Learning

In recent years, there has been a significant increase in the variety and number of skincare products provided by companies. Having too many options makes it overwhelming for customers to identify which product is right for them when they shop for skincare products in-store or online. With the rise of online social sites, people now have access to information and product reviews freely shared by similar users to help in their decision making. Forum websites like Reddit, and online retail websites such as Amazon have a massive amount of user reviews where people express their opinions about products and services.

In this project, we aim to leverage the rich and valuable knowledge contained in online reviews to develop personalised skincare recommendations. Personalised recommendations can help customers find the right product, save time and improve their shopping experience while at the same time assisting the brands to increase their sales and conversion rates.

## Skincare Recommendation Engine Methodology
The recommendation system learns to model users and item interactions for collaborative filtering using text reviews. In order to develop the model, the following assumptions were made:
1. User-written reviews may be used to represent items and users.
2. The user reviews may imply the user’s preferences for the item under discussion.

As a result of this, we formulated a three-step approach:
1. Identify the topics mentioned in the reviews.
2. Perform sentiment analysis to derive user ratings inferred from sentiment scores.
3. Model user and item interaction using a deep neural network.

### Data Collection 
In this project, we selected three datasets to develop the skincare recommendation system. The primary dataset is user comments from Reddit.com (r/SkincareAddiction subreddit), the second dataset is a skincare ingredient dictionary scraped from a trusted database, and the third is a list of skincare product scraped from Boots.com. All three datasets were ethically sourced.

### [Data Pre-Processing](https://github.com/luhlitt/Skincare-Recommendation/blob/main/text_pre_processing_%26_user_item_matrix_creation_recommender_system.ipynb)
Transforming text in natural language format to numeric representations is a critical component of the proposed methodology.
The concept of how to use text user reviews was by investigating what products/ingredients were mentioned in the user review. We extracted product keywords from text user reviews to represent products by matching product keywords to a set of predefined products/ingredients.

Afterwards, we did sentiment analysis to derive scores that would serve as user ratings. 

### Algorithms performed
1. [Matrix Factorisation](https://github.com/luhlitt/Skincare-Recommendation/blob/main/NCF_%2B_reviews.ipynb)
1. [Neural Collaborative Filtering](https://github.com/luhlitt/Skincare-Recommendation/blob/main/NCF.ipynb)
1. [Neural Collaborative Filtering + Topics](https://github.com/luhlitt/Skincare-Recommendation/blob/main/NCF%20%2B%20topics.ipynb)
1. [Neural Collaborative Filtering + Reviews](https://github.com/luhlitt/Skincare-Recommendation/blob/main/NCF_%2B_reviews.ipynb)

### Conclusion and Next Steps

This project proposed a methodology to skincare recommendation, which has the capability of using text user reviews as the primary source of recommendation knowledge. It is therefore not based on static user-profiles and item catalogues, both of which might not be available in realistic settings. The main components of the system include cleaning of reviews, feature extraction, and using a deep neural network for rating prediction. Based on experimental results, it can be concluded that effective mining of user reviews can reveal some information about customer preferences. 

This system deployed in an e-commerce setting can help narrow customer choice, predicting the products most likely to be purchased by the customer, thus increasing business sales & brand loyalty.

### References
1. Esparza, S.G., O’Mahony, M.P. and Smyth, B. (2012) [‘Mining the real-time web: a novel approach to product recommendation'.](https://dl.acm.org/doi/10.1016/j.knosys.2011.07.007)
1. McAuley, J. and Leskovec, J. (2013) [‘Hidden factors and hidden topics: understanding rating dimensions with review text’.](https://cs.stanford.edu/people/jure/pubs/reviews-recsys13.pdf)
1. Chen, L., Chen, G. and Wang, F. (2015) [‘Recommender systems based on user reviews: state of the art’.](https://dl.acm.org/doi/10.1007/s11257-015-9155-5)
1. Zheng, L., Noroozi, V. and Yu, P.S. (2017) [‘Joint deep modelling of users and items using reviews for recommendation’.](https://arxiv.org/abs/1701.04783)
1. Shoja, B.M. and Tabrizi, N. (2019) [‘Customer Reviews Analysis With Deep Neural Networks for E-Commerce Recommender Systems’.](https://ieeexplore.ieee.org/document/8813018)
1. Zhang, S., Yao, L., Sun, A. and Tay, Y. (2019) [‘Deep learning based recommender system: A survey and new perspectives.](https://dl.acm.org/doi/10.1145/3285029)
1. Srifi, M., Oussous, A., Lahcen, A.A. and Mouline, S. (2020) [‘Recommender Systems Based on Collaborative Filtering Using Review Texts—A Survey’](https://www.mdpi.com/2078-2489/11/6/317)
