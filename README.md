i3
==

My configuration file for i3 Window manager in Debian Jessie.


### Touchpad Settings
To enable different settings for touchpad, edit the synaptics configuration file in `/etc/share/X11/xorg.conf.d/50-synaptics.conf` as follows:

    Section "InputClass"
            Identifier "touchpad catchall"
            Driver "synaptics"
            MatchIsTouchpad "on"
            # To enable single click
            Option "TapButton1" "1"
            # To enable double-click
            Option "TapButton2" "2"
            Option "PalmDetect" "1"
    EndSection
    
    
