# Spotify_Billboard_Hit_Prediction
SONG HIT PREDICTION: PREDICTING BILLBOARD HITS USING SPOTIFY DATA
# Introduction
The Billboard Hot 100 is the standard record chart for songs in the United States, published weekly by Billboard magazine. In the United States, chart rankings are based on physical and digital sales, radio play, and internet streaming.

In this project, I have attempted the Hit Song Science (HSS) problem, which aims to predict which songs
will become chart-topping hits. The underlying assumption
in HSS is that hit songs are similar with respect to their features. 
Musicians, labels, and retailers benefit from hit prediction because successful songs generate more cash and allow artists to reach a broader audience. If a label wants to boost earnings, it could decide to spend its limited resources (advertising, studio equipment, etc.) on tunes that are likely to become successful. On the other hand, if an artist wishes to project a non-mainstream musical style, he or she may opt to produce tunes that are unlikely to become popular.
# Dataset and Features
To construct the final dataset of songs, I followed these steps:
1) Downloaded a sample of 19000 songs from Kaggle,containing both billboard hits and non hits.
2) Scraped songs from the Billboard API , which contained the Billboard hits of every week from the year 1990-2020.
3) Merged the dataset from step 1 and 2.
4) Extracted 16 features of songs from above dataset using the Spotify Web API.

The features were as follows:

**Context**: Liveness, Acousticness

**Mood** : Danceability, Valence, Energy, Tempo

**Properties**: Loudness, Speechiness, Mode, Key, Instrumentalness, Explicit, Duration, Time Signature, Release year, Popularity

The final dataset after pre-processing and cleaning had around 18.5K rows.

# EDA
![heat_map](https://user-images.githubusercontent.com/66065738/149577551-ac4c6f90-7727-4bc1-a667-e3104ba24b41.png)
![song release each year](https://user-images.githubusercontent.com/66065738/149577554-a9088a2e-9108-4a04-a092-48945235a2c8.png)
![Characterstics of features over a period](https://user-images.githubusercontent.com/66065738/149577564-2fcff73c-db6f-4cff-8472-3e5e5f0f4ea9.png)
![Top20 Billboard hits](https://user-images.githubusercontent.com/66065738/149577558-8ddcfcc8-6f59-4678-9ca0-f7466ed494b1.png)
![Top Artist of each year](https://user-images.githubusercontent.com/66065738/149577556-1dd7d205-3009-418a-a4a2-34016a354f3a.png)
![distplot](https://user-images.githubusercontent.com/66065738/149577541-746d73a3-4ad6-4d4e-a4cb-31407eefd50c.png)
![boxplots](https://user-images.githubusercontent.com/66065738/149577562-2ae19921-c5b5-4b12-a4a4-bae27fde36a2.png)
![image](https://user-images.githubusercontent.com/66065738/149578560-78439a6b-aa06-4382-a7ba-f34cf786e451.png)

# Models & Results:
**Random Forest**: This model yielded an accuracy of 82.5% on the test dataset. The confusion matrix for the results is shown below:

![image](https://user-images.githubusercontent.com/66065738/149578392-6a65d89e-d5fe-492c-af4e-4917fbd80e43.png)

# References:
https://www.kaggle.com/edalrami/19000-spotify-songs
https://spotipy.readthedocs.io/en/2.19.0/
https://developer.spotify.com/documentation/web-api/reference/#/operations/search
https://towardsdatascience.com/a-practical-guide-to-exploratory-data-analysis-spotify-dataset-d8f703da663e
https://www.statisticshowto.com/probability-and-statistics/skewed-distribution/
https://en.wikipedia.org/wiki/Billboard_Hot_100
https://developer.spotify.com/discover/
