# Music Recommendations
This project consists of scripts each dedicated to recommending music in some way. Currently I only have a script for finding artist recommendations and creating a playlist out of them. In the future, I'd like to make a script leveraging the Last.FM API to recommend similar artists.

## Artist Song Recommendations
The `recommend_artists.py` script grabs each given artist's top 3 songs and 3 random songs, then creates a playlist out of the pulled songs.

The file accepts 0 to 2 arguments:
- 0 args: uses default values
- 1 args: uses same value for both number of popular songs and random songs
- 2 args: uses first and second value for each value respectively
```bash
$ python3 recommend_artists.py
$ python3 recommend_artists.py 3
$ python3 recommend_artists.py 3 5
```

Once you run it, you will be asked which artists you'd like to be recommended from and then what you'd like to name the playlist. Once it finishes running, you'll have a new playlist