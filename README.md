# myscreensaver
Profile to allow the end user to save a jpg (myscreensaver.jpg) in a standard location /userhome/myscreensaver/myscreensaver.jpg so they can change their screensaver at will.  
A a little exercise to see about helping Martijn van Tricht
* Multiple files can be saved in the /userhome/myscreensaver directory but only myscreensaver.jpg will persist after a reboot
    * This behavior can be modified by removing the rm -rf /wfs/user/myscreensaver section in the firmware customization section of the profile. It's not pretty but it works.
    * This may also require a re-location of /wfs/user/myscreensaver to some larger place like /custom. I'll leave that up to the engineer
* The browser will need to be configured to ask the user where to download files if this is the direction they want to take
    * Of course, the /wfs/user/myscreensaver file can be populated with other methods too, like wget or curl on boot.
