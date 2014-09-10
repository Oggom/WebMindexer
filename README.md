WebMindexer
===========
WebMindexer v2.15 Download:<br>
https://github.com/neojam/WebMindexer/releases





[Demonstration:](http://a.pomf.se/lmxjus.webm)

[![Alt text for your video](http://img.youtube.com/vi/T-D1KVIuvjA/0.jpg)](http://a.pomf.se/lmxjus.webm)


What it does:
=================================================================  
- WebMinDEXER will create "_thumbs" subfolders in all your folders that contain WebM files.
- WebMinDEXER will generate  JPG-previews (with FFMPEG) of your WebM videos and save it in "_thumbs" subfolders
- WebMinDEXER will create HTML files with links to your Webms and created jpg-previews


How it does it:
=================================================================  
With help of
FFmpeg (http://ffmpeg.zeranoe.com/builds) and <br />Fancybox (http://fancyapps.com/fancybox/)


How to:
=================================================================  
- Start the WebMinDexer.exe
- then either Left-Click on the tray icon 
  or right click the  tray icon and select "Index a WebM-Folder and Its Subfolders"
- Select ANY file
- Wait till WebMinDEXER and FFmpeg are done generating webpages and images
  (html pages will be generated first/faster, but you'll need to wait for FFmpeg-CMD-window to close.
   once it closed, it means all thumbnail Images were created)

Note:
If you run WebMinDEXER later again, it will update html pages, but existing JPG files wont be updated.
WebMinDEXER will only create missing JPG files of your new vids.

If at any point later, you decide to delete any of your WebM-folders, this deleted folder will still be visible on the OMNI-Page.
You'll need to either delete the according HTML pages from "..\WebMinDEXER\INDEXED\HTML", or you can right click 
the WebMinDexer's tray icon and select "Delete all created HTML-pages", but this will delete ALL html pages, even of existing
WebM folders (youll need to reindex the folders again, to fill the OMNI-Page).




Keyboard-Keys for viewing Videos <br>(works best in Mozilla Firefox, once you clicked on video-thumbnail) :
==================================================================================================
next:               right arrow, page down,  down arrow, enter<br />
prev :              left arrow, page up, up arrow, backspace<br />
close:              escape key<br />
Slideshow:          space (start/stop slideshow)<br />
toggle fullscreen:  f<br />



If videos appear too large after you clicked on a thumbinail:
=================================================================  
- Go into "xCSS" folder
- browse to desired resolution folder (for example in: "1280x720" folder) 
- and copy "jquery.fancybox.js" and "jquery_001.js" into "xCSS" folder

Or you can manually change sizes in files:
jquery_001.js: lines 19-20
jquery.fancybox.js: lines 59-60


To change the speed of slide-effect of prev/next videos:
================================================================= 
change value of "openSpeed","prevSpeed", "nextSpeed" parameters in "jquery.fancybox.js" at lines 152-172


To change the duration per video in slideshow mode:
================================================================= 
change value of "playSpeed" parameter in "jquery.fancybox.js" at line 87 (ex. 5000 is for 5 seconds)




Notes
================================================================= 
WebMinDEXER is still buggy and does not support folders/files with unicode characters.
To be safe, for now use english letters and numbers only, when naming your WebM files and folders.
