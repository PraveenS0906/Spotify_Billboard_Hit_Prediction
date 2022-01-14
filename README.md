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



