# Our Team Project [Dating App: LOOK AT ME](https://github.com/yayapa/SDAPraktikum/tree/main/E2)

This is a project that has been implemented as part of [the Coding da Vinci Hakathon](https://codingdavinci.de/) and uses this [data set](https://codingdavinci.de/daten/look-me-100-gesichter-100-geschichten) from the Augustinermuseum. Our project can be split into three use cases:

  1. Style Transfer
  2. Similarity
  3. Exploration



## Similarity Model Description

I adapted the unsupervised learning method to cluster portraits. The trained-well clustering model was stored in a pickle file. 

These portraits were clustered into eight groups and stored in a pickle file. When a user uploads a new picture by GUI, we exploit the similarity and make a reliable prediction that portraits in which cluster has the highest similarity with this new picture.

The details are as follows:

1. Extract the features of each portrait;
2. Apply the k-means algorithm to process the feature matrix and form a robust clustering model;
3. Use this model and predict function to decide a new picture belongs to which cluster;
4. Return all the portraits in this cluster.

How to use it?

1. Run the requirements.txt and import all the necessary packages;
2. Run the cluster function to train a model;
3. Run the prediction function to get the most similar portraits.
