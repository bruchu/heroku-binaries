heroku-binaries
===============
Vulcan builds to be used on heroku

ffmpeg.tar.gz - x264, mp3lame, libvorbis, libogg (also includes ffmpegthumbnailer). You can install using https://github.com/bruchu/heroku-buildpack-ffmpeg (and multi buildpacks) or if you extract manually, make sure that the LD_LIBRARY_PATH is set:

    $ export LD_LIBRARY_PATH="$LD_LIBRARY_PATH:vendor/ffmpeg/lib:vendor/faac/lib:vendor/libogg/lib:vendor/libvorbis/lib:vendor/mp3lame/lib:vendor/x264/lib"
