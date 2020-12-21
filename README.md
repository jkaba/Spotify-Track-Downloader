# Spotify Downloader
A script written in Python that extracts song or playlist information from Spotify and downloads them from YouTube if found.

This README would normally document whatever steps are necessary to get spotify-dl up and running.

### What is this repository for? ###

* spotify-dl allows you to download spotify songs or playlist
* This repo contains spotify-dl source code

# How to Install ?
To use the spotify downloader, you will need to have the following packages installed :
  * bs4
  * youtube-dl
    
# How to use ? (Basic Form)
Either using your own spotify account or downloading a single song or playlist by providing an ID , ex:
The following command will download the song and save it as an mp3 file

    $ ./spotify-downloader --track {spotify_song_id} --dl youtube --access_token <your_access_token>
    
You can get the song ID by getting the spotify URI of the song
{spotify_song_id_ex} : 28Ct4qwkQXY2W5yyNCLuVI

You can generate an access token with the command below:

    $ ./spotify-downloader --gen_url 
    
You will also need to create an application on https://developer.spotify.com/

In the code change the following with your info:

    CLIENT_ID=""
    CALL_BACK_URL=""
