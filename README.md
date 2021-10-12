# i3-gaps-installation

**First, lets update the system :**

`sudo apt update && sudo apt upgrade`

**Then, i3 and the basic utilities :**

```sudo apt install i3 i3status suckless-tools libxcb1-dev libxcb-keysyms1-dev libpango1.0-dev libxcb-util0-dev libxcb-icccm4-dev libyajl-dev libstartup-notification0-dev libxcb-randr0-dev libev-dev libxcb-cursor-dev libxcb-xinerama0-dev libxcb-xkb-dev libxkbcommon-dev libxkbcommon-x11-dev autoconf xutils-dev libtool automake libxcb-xrm-dev```

**Then logout and login with i3 selected as your desktop (in XFCE this will be the burger menu at the top of the login screen)
When i3 prompts you to create a configuration file say yes, if you said no, you can simply run :**

`i3-config-wizard`

**Then install i3-gaps :**

`sudo apt install i3-gaps`

**To activate the gaps you will need to add them to your config.
Open ~/.config/i3/config in a text editor and add these lines :**

```
# this is where you set the gap width between your windows
gaps inner 5
# this is where you set the gap width between the screen border and your windows
gaps outer 5

# this will remove the border on all windows
for_window [class="^.*"] border pixel -1
```

**And that's it, you're done!**
