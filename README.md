# Spotify decades classification 
Building a classifier for songs on Spotify that guesses what decade is a song from using Spotify audio features.
1. Obtaining data from Spotify Web API (Spotify_decades_get_data.ipynb)
  I chose seven Spotify playlist, each containing songs from one decade, specifically 
  All out 50s https://open.spotify.com/playlist/37i9dQZF1DWSV3Tk4GO2fq;\n
  All out 60s https://open.spotify.com/playlist/37i9dQZF1DXaKIA8E7WcJj;\n
  All out 70s https://open.spotify.com/playlist/37i9dQZF1DWTJ7xPn4vNaz;\n
  All out 80s https://open.spotify.com/playlist/37i9dQZF1DX4UtSsGT1Sbe;\n
  All out 90s https://open.spotify.com/playlist/37i9dQZF1DXbTxeAdrVG2l\n
  All out 00s https://open.spotify.com/playlist/37i9dQZF1DX4o1oenSJRJd\n
  All out 10s https://open.spotify.com/playlist/37i9dQZF1DX5Ejj0EkURtP\n
  and scraping audio features for every song in those playlist (i.e. danceability, energy, key, loudness, mode, speechiness, acousticness, instrumentalness, liveness, valence and   tempo) and saving this data as csv file.
2. Building a model (Spotify_decades_classification.ipynb)
   Using audio features as input and decade as output of classification, performing data exploratory analysis, feature engineering using Random Forest Classifier and ensamble        models with RFE resulting in choosing only 6 features to build Logistic Regresion, Random Forest Classifier and Gradient Boosting models alongside with grid searching for best    models parameters
