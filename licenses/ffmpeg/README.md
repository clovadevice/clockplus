# ffmpeg 

# How to build

1. Download the ffmpeg
   ```
   wget https://ffmpeg.org/releases/ffmpeg-4.1.3.tar.bz2
   ```

3. Build
   ```
   tar xf ffmpeg-4.1.3.tar.bz2
   cd ffmpeg-4.1.3/
   ./configure --disable-everything --enable-swscale --enable-swresample --enable-decoder=aac* --enable-decoder=flac --enable-decoder=mp3* --enable-decoder=pcm* --enable-decoder=vorbis --enable-demuxer=aac* --enable-demuxer=flac --enable-demuxer=mp3* --enable-demuxer=ogg --enable-demuxer=mov --enable-demuxer=wav --enable-demuxer=hls --enable-demuxer=mpegts --enable-filter=aformat --enable-filter=aresample --enable-filter=volume --enable-filter=afade --enable-filter=anequalizer --enable-protocol=crypto --enable-protocol=file --enable-protocol=hls --enable-protocol=http* --enable-pic --enable-shared --enable-openssl --enable-decoder=amrnb
   make
   make install
   ```
