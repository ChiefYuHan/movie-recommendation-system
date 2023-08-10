# Movie Redommendation System(s)

We load our datasets from a Github directory: https://github.com/ChiefYuHan/movie-recommendation-system/tree/main.

The original dataset was downloaded from Kaggle: https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset

We implemented three different approaches to a movie recommendation system.
1. KNN
2. Similarity Learning (Collaborative Filtering)
3. Deep Learning 

# 1. KNN
Here is the link to Google Colab: https://colab.research.google.com/drive/14q4tzpp7bq-kxv3fu7dNUfHUy2ycVv79?usp=sharing

## How to run it?
1. Run the entire Code
2. Run this method `get_mr_by_genre(userId, genre)` to get movie recommendations for the user ***userId*** of ***genre***.

**Attention**: Since we sample a subset of all userIds in the beginning, execute `print(rand_userIds)` to see which userIds you can use:

![image](https://github.com/ChiefYuHan/movie-recommendation-system/assets/75226168/34520211-88d8-4818-9185-ad82af07c7d9)

The knn algorithm will also not be able to calculate a distance if the user has not rated movies of the specified genre yet. Use the method `get_user_genre_list(userId)`to find out, given a ***userId***, which genres the user has already rated:

![image](https://github.com/ChiefYuHan/movie-recommendation-system/assets/75226168/2b4097aa-6009-446f-8de2-f15cedcb3fc2)

If executed correctly, the output will look something like this:

![image](https://github.com/ChiefYuHan/movie-recommendation-system/assets/75226168/71e9250f-e099-40b8-b770-ace77d40e0e7)

# 2. Similarity Learning (Collaborative Filtering)
Here is the link to Google Colab: https://colab.research.google.com/drive/1uYyZjPKAZt_aPhkJ-_qW38WIJzFf46f_?usp=sharing

## How to run it?
1. Run the entire Code
2. Run this method `get_mr_by_genre(userId, genre)` to get movie recommendations for the user ***userId*** of ***genre***.

**Attention**: Since we sample a subset of all userIds in the beginning, execute `print(rand_userIds)` to see which userIds you can use:

![image](https://github.com/ChiefYuHan/movie-recommendation-system/assets/75226168/34520211-88d8-4818-9185-ad82af07c7d9)

If executed correctly, the output will look something like this:

![image](https://github.com/ChiefYuHan/movie-recommendation-system/assets/75226168/9e026a12-7840-4891-a1b7-df6cfd136ca9)

The default number of recommendations is 9. Depending on the genre, the number of recommendations may vary (in the case a recommending user has not seen at least 3 movies of the specified genre).

# 3. Deep Learning 
Here is the link to Google Colab: https://colab.research.google.com/drive/156bOlrktKHF8STHXIfUXBnJnIsttEN_3?usp=sharing

## How to run it?
1. Run the entire Code
2. Run this method `get_movie_rec_for_user(userId)` to get movie recommendations for the user ***userId***.

**Attention**: Since we sample a subset of all userIds in the beginning, execute `print(rand_userIds)` to see which userIds you can use:

![image](https://github.com/ChiefYuHan/movie-recommendation-system/assets/75226168/34520211-88d8-4818-9185-ad82af07c7d9)

If executed correctly, the output will look something like this:

![image](https://github.com/ChiefYuHan/movie-recommendation-system/assets/75226168/ea1d9221-1316-4936-9fc6-6e7e1458712c)

Use the method ***already_rated(userId)*** to output a list of movies the selected user has already seen and rated. Often there will be correlations between them and the recommended movies:

![image](https://github.com/ChiefYuHan/movie-recommendation-system/assets/75226168/61aabe79-0698-403e-9094-fd6a3b803443)


