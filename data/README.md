# data

If using an external dataset (that doesn't come in an R package), place data file(s) in this folder.

Then, include metadata about your dataset including information on provenance, codebook, etc.

The codebook for your data file(s) using the following format.

## billboard.csv

|variable               |description |
|:----------------------|:-----------|
|url (chr)              | Billboard chart URL |
|week_id (chr)          | week ID, in form MM/DD/YYYY|
|week_position (num)    | position of song for that week (1-100) |
|song (chr)                  | song name |
|performer (chr)              | performer name |
|song_id (chr)         | song ID - combo of song/singer |
|instance (num)              | number of times this song has appeared on the chart |
|previous_week_position (num)  |song's position last week |
|peak_position (num)         | peak position of the song (as of that week) |
|weeks_on_chart (num)        | number of weeks on the chart (including that week) |


## audio_features.csv

|variable                  |description |
|:-------------------------|:-----------|
|song_id (chr)                   | song ID (song name and performer name) |
|performer (chr)                | performer name  |
|song (chr)                   | song name|
|spotify_genre (chr)            | genre of song (often a list of genres)|
|spotify_track_id (chr)         | track ID |
|spotify_track_preview_url (chr) | potify URL |
|spotify_track_duration_ms (num) | duration in ms|
|spotify_track_explicit (bool)    | is song explicit |
|spotify_track_album (chr)       | album name|
|danceability (num)             | (0.0 - 1.0) how suitable a track is for dancing (includes tempo, rhythm stability, beat strength, etc) |
|energy (num)                   | (0.0 - 1.0) based on speed, volume, and timbre |
|key (num)                      | estimated overall key of track - ints map to pitches using standard pitch class notation (0=C, 1=C#, 2=D, etc) |
|loudness (num)                 | "loudness" of track, in decibels (dB)|
|mode (num)                     | major=1, minor=0|
|speechiness (num)              | (0.0 - 1.0) amount of spoken words (ex: podcast would be closer to 1, orchestral music would be closer to 0) |
|acousticness (num)             | (0.0 - 1.0) Confidence measure of whether track is acoustic|
|instrumentalness (num)       | predicts whether track contains no vocals (0.0 - 1.0, values closer to 1.0 are more instrumental) |
|liveness (num)                | detects presence of an audience in recording (0.0-1.0, values above .8 indicate strong likelihood of live track) |
|valence (num)                  | (0.0 - 1.0) quantifies musical positivity of the song |
|tempo (num)                    | tempo in BPM |
|time_signature (num)            | time signature |
|spotify_track_popularity (num) | (0 - 100) popularity |
