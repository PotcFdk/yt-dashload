yt-dashload
===========

A small frontend for downloading high quality videos with [youtube-dl](https://github.com/rg3/youtube-dl/).

It always chooses the best quality available (the *really* best one - youtube-dl currently only goes as far as 720p since everything above that uses DASH and thus provides separate video and audio streams).

It does this by downloading the best video and audio streams provided separately and then uses ffmpeg to merge them into one file.

### Dependencies
- installed ffmpeg (avconv support: currently not necessary in my use cases, if you need it, [create a new issue](https://github.com/PotcFdk/yt-dashload/issues) so I see that it's actually needed and that I should implement it)
- a recent copy of [youtube-dl](https://github.com/rg3/youtube-dl/) (just drop the executable into the same directory as this script)


### Usage
$ ./yt-dashload [YouTube video url]
