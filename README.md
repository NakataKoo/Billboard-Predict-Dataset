# Billboard-Predict-Dataset
Dataset for Billboard charting predictions.
## Overview
This dataset includes a comprehensive collection of songs from the US market, released between 2000 and 2020, obtained using the Spotify and Billboard APIs. The dataset contains 15,951 tracks, with a focus on analyzing the characteristics that may influence a song's success in the Billboard charts.

## Data Description
The dataset is in CSV format and includes 214 columns, covering a range of features such as:

- release_date: The number of days since the song's release, a continuous variable.
- length: The duration of the song in milliseconds.
- explicit: A boolean variable indicating whether the song contains explicit lyrics.
- followers: The number of followers on Spotify of the artist at the time of data retrieval.
- Spotify's unique audio features like danceability, acousticness, energy, instrumentalness, liveness, loudness, speechiness, tempo, time signature, valence.
- Availability in different markets represented by boolean variables for each country code (e.g., US, JP).
- title language: A categorical variable that represents the language of the title.
- title length: A continuous variable that represents the number of characters in the title.
- lyrics language: A categorical variable that represents the language of the lyrics.
- non diatonic rate: A continuous variable that represents the non-diatonic chord rate.
- n chord type: Continuous variable that represents the number of chord types.
- lyrics sentiment: Continuous variable that represents the result of sentiment analysis on lyrics.
- lyrics topic: A continuous variable representing the probability of being included in each topic using the result of topic analysis with the number of topics as 9. (For example, if the probability of being topic 1 is 0.1, then topic 1 = 0.1, which is obtained for each song from topic 1 to topic 9 for each music piece, and each is added as a separate continuous variable).
- key signature sin: The value of sin when the type of key signature is obtained from the key and mode of the music, and the type of key signature is expressed by a trigonometric function based on the five-degree circle.
- key signature cos: The value of cos when the type of key signature is expressed by trigonometric functions in the same way as described in the key signature sin.
- Target Variable "ChartIn": A binary variable indicating whether the song has charted in the Billboard Hot-100 (1 for charted, 0 for not charted).

## How to Use
1. Download the dataset from this repository.
2. Import the dataset into your data analysis tool of choice.
3. Utilize the dataset for music industry trends analysis, predicting Billboard chart success, or other related research.

## Data Collection Methodology
Acoustic, charting, and lyrics data were systematically collected using Spotify and Billboard and Genius APIs.

The data was also obtained from Chordify by scraping the chord progression information into features.

This dataset was balanced for the distribution of songs over the years. Audio features, metadata from Spotify, chart information from Billboard, and other derived features were combined to create a comprehensive analysis tool.

## Limitations and Ethics
This dataset primarily represents the US market and focuses on popular tracks, which might not reflect global music trends. Ethical considerations should be taken when using follower count as a measure of popularity.

## Ackowledgements
Special thanks to Spotify, Billboard and Genius for providing the APIs to access the data.
