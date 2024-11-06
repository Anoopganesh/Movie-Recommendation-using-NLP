# Movie-Recommendation-using-NLP
Recommendation System
A recommendation system is a system that filters all the videos or movies based on our preferences and our watch history and provides recommendations to the users.

Let us build a recommendation system.

Dataset
Before processing further, we need a dataset to work on.

This dataset contains two CSV files. One is credits, and the other is a movie file. We will explore these files later. This file contains columns like budget for the movie, genres, homepage, id, keywords, original_language, original_title, overview, popularity, production_companies, production_countries, release_date, revenue, runtime, spoken_languages, status, tagline, title, vote_average, vote_count.

The file contains columns like title, cast, and crew in credits.

Tools and Libraries used
Python – 3. x
Pandas – 1.2.4
Scikit-learn – 0.24.1
Command used to install the libraries is

pip install pandas scikit-learn
To install the packages following code is used

import numpy as np
    import pandas as pd
    import matplotlib.pyplot as plt
    from sklearn.feature_extraction.text import TfidfVectorizer
    from sklearn.feature_extraction.text import CountVectorizer
    from sklearn.metrics.pairwise import linear_kernel
    from sklearn.metrics.pairwise import cosine_similarity
    from ast import literal_eval
A recommendation system is either a program or an algorithm for which the input is the watch history, search history, etc.. and analyses the genre, cast, director, and so on, and based on this analysis, some movies are recommended for the users, That is how the recommendation system works either for a product selling platform like Amazon, Myntra, Flipkart, or for an OTT platform like Netflix, Amazon prime Video, Aha, and so on.

Types of Recommendation System
Generally, there are three types of recommendation systems.

1. Demographic filtering

2. Content-based filtering

3. Collaboration-based filtering

Let’s see them one by one.

Demographic filtering: In this, the recommendations are the same for every user despite their interests. For example, let’s take the top trending movies column in ott platforms. These are the same for every user. Demographic filtering is the system behind it.

Content-based filtering: Filterings are based on movie metadata. Metadata contains details like movies, songs, products, etc. Based on this data, the system will recommend related movies so the user will like them.

Collaboration-based filtering: Here, the system will group users with similar interests and recommend movies to them.
