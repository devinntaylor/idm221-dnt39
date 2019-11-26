#FTP Software
- Cyberduck

#Media Types

- MPEG
- AVI
- MP3
- AAC

###Plugins 
- Quicktime plugin 

###Video Codecs
- H.264 
    - same thing as MPEG
- Theora
- VP8

#What's Happening
- Determine media type 
- Can it decode the video / audio? 
- Decode / display the video
- Decode and play the audio
- Interpret metadata

caniuse.com

###HTML5 

#Encoding Media 
- Miro Converter ***
    - Drag and drop video / audio 
- iTunes (audio)
- Quicktime Pro (video/audio)
- Windows Media Encoder
- Adobe Media Encoder
- FFmpeg
- Handbrake

#HTML Code
    <video src="media/myvideo.mp4"></video>
    <audio src="media/myaudio.mp3"></audio>

    <video width="1280" height="720" controls autoplay poster="media/myvideo_poster.jpg">
        <source src="media/myvideo.mp4" />
        <source src="media/myvideo.webm" type="video/webm" />
        <source src="media/myvideo.ogv" type="video/ogg" />
    /video>

    <audio controls autoplay>
         <source src="media/myaudio.mp3" />
         <source src="media/myaudio.ogg" />
    </audio>

###Options: 
src
poster
preload
autoplay
loop
muted
controls
width
height

<details> element with summary and pararaph = accordian style paragraph  