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
