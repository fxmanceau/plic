# Plic - Music Player
> A custom music player modular with JSON database

## Features
- Basic music player controls (play/pause, previous/next music, seekbar and volume bar)
- Display current time and audio duration
- Controls like Spotify (random music, play in loop, play the same music)
- Advanced behavior for the controls :
    - Drag seekbar and volume bar when mousedown on the dot or on the bar

    - Clicking on volume icon toggles mute or unmute action. When muted, the volume is saved

    - Next music button triggers play music

    - Previous music puts currentTime 0 if the music has been played for less than 5s, else it triggers play music

    - If Loop button is not activated, then the music is paused when it is ended and currentTime is to 0

    - If Loop button is on playlist-loop, the next music is automatically played

    - If Loop button is on music-loop, the same music is played continuously

    - If Random button is activated, the Loop-button behavior is mixed with it

- Random button, if activated, creates a random playlist and we can navigate in it with previous and next buttons (the random order remains)
- Two main colors are created by analysing, with canvas, Data URI of the album cover image
- Lyrics (.vtt files) synchronized with the music (using track HTML tag)
- Favicon
- The Title of the page is the music is played, and is the default one when not played
- Android notification with embedded controls, music name and artist
- Keyboard shortucts (spacebar to play, ctrl + left arrow to play previous music, ctrl + right arrow to play next music)
- CSS Animations to change and display images, musics informations and lyrics
- JSON database to add easily musics, (get it with fetch)
- Full responsive (desktop, mobile and tablet) :
    - Seekbar and volume bar draggable with touchevent

    - Lyrics remains displayed

    - Portrait and landscape modes supported

- LocalStorage enabled :
    - Save automatically the current time, the volume, the music played, and the loop/random states

    - If Random button was activated before the refresh, the random playlist is saved with the music played (we can navigate in it after refreshing)
    
- Minimifed JS and CSS
- Compressed images
- SASS
- Custom font for the icons, not images!

## Resources
- Canvas
- Google Mediadata API
- Spotify controls behavior
- rentanadviser.com for the lyrics
- icomoon.io for the custom font
- reset.css

## Install
- Use a web server or MAMP (needed for fetch and lyrics files)
- Or see [here](francoisxaviermanceau.fr/lab/plic)

## Compatibility
### Works on :
- [x] Chrome (Desktop and Mobile devices)
- [x] Safari (Desktop devices)
- [x] Edge (Woohoo incredible :O \o/)

### Works (but without some features) on : 
- [x] Safari (Cannot control volume using the volume bar, functionnality locked by Apple) (Mobile devices)
- [x] Firefox (lyrics doesn't work) (Desktop and Mobile devices)