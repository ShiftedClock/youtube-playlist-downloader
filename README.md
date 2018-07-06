## This is an archived repository.
I recommend using youtube-dl instead: https://github.com/rg3/youtube-dl
It supports downloading playlists using the command line flag --playlist-start, and many other options.

# youtube-playlist-downloader
A Python CLI utility to download an entire playlist from YouTube.
By default it downloads the videos from the [Berkeley Deep Reinforcement Learning class CS294](https://www.youtube.com/playlist?list=PLkFD6_40KJIwTmSbCv9OVJB3YaO4sFwkX).

To run, clone this repository into an empty directory:
 `git clone https://github.com/svass/youtube-playlist-downloader.git`
 
Then install the one dependency:
 `pip install pytube`
 
Finally run the script:
 `python playlist-downloader.py`
 
Optionally specify a playlist url to download:
 `python playlist-downloader.py -p https://www.youtube.com/playlist?list=PLBmH8k4EW7GJ-tsTXJLOKQuNYXpRu8mjS`
 
And/or a destination directory to save the videos in:
 `python playlist-downloader.py -d ~/corgi_videos -p https://www.youtube.com/playlist?list=PLBmH8k4EW7GJ-tsTXJLOKQuNYXpRu8mjS`
 
The script checks if the videos from the playlist are already in the destination directory.
This means you can re-run the script and only download the newly uploaded content.
