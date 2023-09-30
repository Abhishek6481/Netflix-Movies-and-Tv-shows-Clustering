# Netflix-Movies-and-Tv-shows-Clustering
![--------------------------------------------------------------------------------------------](https://github.com/andreasbm/readme/blob/master/assets/lines/grass.png)

### This repository contains the and dataset and the research notbook consisting various aproches for clustering movies and tv shows for netflix dataset. The movies and tv shows are present in the dataset which where released during the period of 1925 to 2021.
![--------------------------------------------------------------------------------------------](https://github.com/andreasbm/readme/blob/master/assets/lines/grass.png)

![N|Solid](https://media.tenor.com/twG41IiAAscAAAAC/no.gif)
# Problem Statement
The dataset we have at hand comprises information about TV shows and movies available on Netflix as of 2019. It was sourced from Flixable, a third-party Netflix search engine.

A fascinating report released in 2018 shed light on some intriguing statistics regarding Netflix's content offerings. According to the report, the number of TV shows on Netflix had nearly tripled since 2010, while the number of movies had decreased by over 2,000 titles during the same period. This highlights a significant shift in the platform's content landscape, with a greater emphasis on TV shows.

Exploring this dataset further presents an exciting opportunity to uncover additional insights. By integrating external datasets such as IMDB ratings and Rotten Tomatoes, we can delve deeper into the quality and reception of the content available on Netflix. This integration opens up avenues to discover compelling findings and gain a more comprehensive understanding of the platform's offerings
# Project Summary 
Netflix is an internet platform that provides streaming services for entertainment. It is a subscription-based service offering a diverse selection of material. The majority of its material is separated into two categories: movies and television shows. In recent years, it has become the most popular OTT platform for individuals all over the world. Customers can, however, terminate their memberships at any moment. As a result, the firm must keep consumers interested in the platform and not lose them. This is where recommendation systems come into play, as offering useful ideas to consumers is critical.

Furthermore, Netflix is a media distribution corporation. It began with DVD delivery over the mail, but has developed significantly throughout the course of its history. Netflix now focuses on video streaming. others of its material is licensed, while others is created in-house.

Netflix first concentrated on movies, but television series are likely to be a more popular genre nowadays. Netflix operates on a subscription basis, with customers receiving unlimited access to material for a fee.

In this project, we'll be working with Netflix data to understand the most recent trends and get insights into the material presented; the dataset was obtained via Flixable, a third-party Netflix search engine. In 2018, they published an intriguing analysis revealing that the amount of TV series available on Netflix has nearly quadrupled since 2010. Since the number of movies on the streaming service has reduced by almost 2,000 titles since 2010, but the number of TV series has nearly quadrupled, a suggested system was long overdue. To deliver it, we will evaluate the data and cluster comparable material by matching text-based attributes through the development of a recommendation engine.

We completed the following project steps:

Getting a sense of the dataset by extracting the head and tail

Obtaining the mean, minimum, maximum, and data types of the columns from the dataset's description

Extraction of data information to show the non-null count of column values

Counting the number of distinct values in each column

Obtaining the form of the, that is, the number of rows and columns

There are null values in the director, cast, nation, release year, and rating columns.

The null values in the column country were filled by mode, and the null values in the cast column were replaced with 'No Cast'.

Plotting relevant graphs to extract information from them.

Then, for NLP, we performed text pre-processing: Tokenization is the process of dividing natural language text into bits of information that may be regarded separate parts. Token occurrences in a document can be utilized as a vector directly representing that document.

B) Punctuation Removal: The text's punctuation is eliminated.

C) Stopword Removal: Stopwords are common words that contribute very little or no substantial information to the text being analyzed. This saves time and minimizes computational complexity.

D) Word Stemming: Word stemming is the process of reducing inflected words to their word stem, base, or root form, which is usually a written word form. This decreases the number of various variants of the same word with the same basic meaning. It is important to remember that stemming does not eliminate.

Then we implemented clustering models like:

K-means Clustering

Agglomerative Clustering

We need to input the number of clusters for the algorithm to cluster in K-means, therefore we used the Elbow technique, Silhouette Score, and Dendogram to determine the number of clusters.

K-means was the most effective algorithm.

We created a recommendation system using the clusters produced by K-means clustering, which provided perfect recommendations for a feature input.

In the end, we effectively did EDA and delivered critical findings to tackle significant business challenges, and the models performed exceptionally well given the data's irrelevance and bulk.
### Data Source:
- [Dataset](https://drive.google.com/file/d/17ecyUUnRHmssQzebQjnW7IUjKrRTC4oI/view?usp=sharing) - Dataset taken from AlmaBetter
# Conclusions for Machine learning models
1. The Elbow graph allowed us to count the number of clusters, which came to be 18. By searching for a strong bend in the curve or a considerable departure from a straight line, this number was found. To find the value signifying the number of clusters, we choose this point on the x-axis.
2. we used Silhouette score method and After evaluating the Silhouette Score, we found that the best score was achieved with 15 clusters, which amounted to 0.0.010383798598527266.
4. We determined the longest vertical distance that may be drawn without crossing any other horizontal lines by evaluating the dendrogram. The number of vertical lines it crossed after passing through this distance was noted. We discovered that 15 clusters is the optimum number for K-means from the dendrogram's point of view.
5. Users of Netflix can organize similar content tastes by clustering text-based features. By seeing patterns and providing tailored recommendations, well-formed clusters improve the recommendation system. This enhances platform user experience and content relevance.




