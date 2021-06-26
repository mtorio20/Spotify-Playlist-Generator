In order to use the main program, you must have 3 items entered into the secrets file:\
-A spotify account user id must be entered in for spotify_user_id(),\
-An authorization must be obtained from Spotify's developer console (https://developer.spotify.com/console/post-playlist-tracks/) Keep in mind OAuth Tokens from spotify expire every 30minutes-1 hour. If playlists are not generating songs correctly, make sure playlist-modify-public or playlist-modify-private are enabled when obtaining a token\
-Lastly, a lastFM api key must be generated https://www.last.fm/api\
\
The main program essentially takes in an artists name from the user and LastFM's API is utilized to generate the top 10 songs of the specified artist and their associated song uris. The uris are then used by Spotify api to create a playlist with the songs.
