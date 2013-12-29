#showtime
This is a simple automator workflow to prepare a Mac for PowerPoint and media playback. The script does the following:

- Quits a selection of applications (configurable) 
- Disables [GeekTool](http://projects.tynsoe.org/en/geektool/)
- Replaces current desktop background with a plain black one
- Disables Notification Centre and Growl
- Hides desktop icons
- Stops Dropbox
- Disables Wifi

Then it will restore to your previous state when you are done.

##Installation
Copy `black-background.jpg` to the `Pictures` folder in your home directory.

The automator scripts can be stored and launched from anywhere on your Mac.

##Configuration
Opening `showtime-start.workflow` in automator will show all the steps in the script.

Any changes in the `showtime-start.workflow` file will also need to be updated in the `showtime-stop.workflow`.

###Closing and Opening Applications
To add more applications to the list. Add the following line in the `Quit Applications` step, changing `Application Name` to the name of the application. E.g `Safari`.

`osascript -e 'tell app "Application Name" to quit'`

![](https://dl.dropboxusercontent.com/u/638291/2013-12-29_17.52.50.png)

###Disable Unused Applications
You will need to disable any steps you do not have installed (E.g GeekTool or Growl) by right clicking on the step. 

![](https://dl.dropboxusercontent.com/u/638291/2013-12-29_17.47.15.png)

##Credits
[Brett Terpstra's Scripting podcast and screencast prep on a Mac](http://brettterpstra.com/2013/12/24/scripting-podcast-and-screencast-prep-on-a-mac/)



