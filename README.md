# Machine Learning Engineer Nanodegree
## Music Classification Model 
## Project: Capstone Proposal and Capstone Project



### Install

This project requires **Python 2.7** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

  

### Code

The code is provided in the `capstone_code.ipynb` notebook file. The `data.csv` dataset file is also needed if there is the desire to run the code on your own enviroment.

**It's recomended to use Jupyter Notebooks for a better visualisation of the code.**
### Run

In a terminal or command window, navigate to the top-level project directory capstone_project/` (that contains this README) and run one of the following commands:

```bash
ipython notebook capstone_project.ipynb
```  
or
```bash
jupyter notebook capstone_project.ipynb
```

This will open the Jupyter Notebook software and project file in your browser.

### Data

The Spotify Song Attributes dataset consists of 2017 data points, with each datapoint having 16 features. This dataset was taken from Kaggle (https://www.kaggle.com/geomack/spotifyclassification). The details from each feature are taken from https://developer.spotify.com/web-api/get-audio-features/ .

**Features**
1. `acousticness`: float, a confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.
2. `danceability`: float, describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable. 
3. `duration_ms`: int, The duration of the track in milliseconds.
4. `energy`: float, a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy.
5. `instrumentalness`: float, predicts whether a track contains no vocals. "Ooh" and "aah" sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly "vocal". The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. Values above 0.5 are intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0.
6. `key`: int, The key the track is in. Integers map to pitches using standard Pitch Class notation. E.g. 0 = C, 1 = C♯/D♭, 2 = D, and so on.
7. `liveness`: float, detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live.
8. `loudness`: float, the overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude). Values typical range between -60 and 0 db.
9. `mode`: int, mode indicates the modality (major or minor) of a track, the type of scale from which its melodic content is derived. Major is represented by 1 and minor is 0.
10. `speechiness`: float, speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks.
11. `tempo`: float, the overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration.
12. `time_signature`: int, an estimated overall time signature of a track. The time signature (meter) is a notational convention to specify how many beats are in each bar (or measure).
13. `valence`: float, a measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).
14. `artist`: string, name of the artist that sings the song.
15. `song_title`: string, name of the song.

**Target Variable**
16. `target`: discrete binary value: 1 for liking a song 0 for not liking