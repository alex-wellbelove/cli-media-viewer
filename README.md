# cli-media-viewer
A very simple solution to the problem of viewing images and videos from elinks and reddit terminal viewer (RTV). 
Currently supports imgur single images and galleries, gfycat, gifv files and youtube. 
Requires feh, urxvt, mpv, elinks. 

## Installation and Usage
Put both mediaswitch.sh and albumview.sh in your path, and use chmod +x. 
For RTV, either change $BROWSER to mediaswitch, or change the browser configuration. 
For elinks, add
> set document.uri_passing.media = "mediaswitch %c >> /dev/null"

to your elinks.conf, and use your defined uri_passing key (Default Alt-O) to load images and videos.
