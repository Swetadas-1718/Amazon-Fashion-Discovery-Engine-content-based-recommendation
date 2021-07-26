# Amazon Fashion Discovery Engine(content based recommendation)
## Why care about product recommendations?
It is estimated that around 35% of the revenues that amazon makes are because of product recommendations. Due to product recommendation bars, as shown above, the user ends up buying a product or two.

- Amazon internally uses two types of recommendation systems:
- 1) Content-Based Recommendation: When we search about polka dot shirts, it uses text and images to recommend similar products.
- 2) Collaborative filtering based Recommendation: 
Imagine, User U1 browsed through products i1,i2,i3
User U2 browsed through i1,i3,i4
Then I can recommend User U3, the product i3 when he is on page i1.
So, this is called a collaborative filtering-based recommendation. Unfortunately, we don't have this data.

- So, in this case study, I used content-based recommendations.

## Overview of the data
- Number of data points/products: 183138
- Number of features/variables: 19
- I used only 6 features out of these 19 features in this workshop.
- I have intentionally not used description as it is lengthy and takes longer time to process.

## Data Cleaning & Understanding
This is extremely important step in machine learning which is often overlooked. The better we understand our data, the more better models we can build.
At the end of data cleaning and preprocessing steps, we already de-duped our data and removed stop words. I was left with 16K products as my dataset.

## Text Based Product Similarity
We worked on :
- Bag of words based product similarity model.
- TF-IDF based product similarity model.
- IDF based product similarity model.
- Word2Vec based product similarity model.
- Average Word2Vec based product similarity model.
- TF-IDF Weighted Word2Vec based product similarity model.
- IDF Weighed Word2Vec based product similarity model.
- Weighed Similarity using brand and color based product similarity model.

- So , we worked on multiple techniques. But, How does real world solution/system built ?
Most companies use multiple techniques or combine multiple techniques and carry out A|B testing to measure the goodness of the models. Of course some business rules are considered.

## Deep Learning based Visual Product Similarity
- Here, I used Convolutional neural networks like VGG-16 to convert my image into dense vector and applied euclidean distance on top of it to bring out the similarity and recommend products. Here VGG-16 converted each image into a 25,088 dimensional dense vector. I got some really interesting results using deep learning.

## Conclusion
- Recommender system can help the user to find the right product.
- It increases the user engagement.
- It helps to make the content more personalized and increases the sales of the company.

## Author
Swetapadma Das
