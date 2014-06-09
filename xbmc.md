# XBMC
Add the following repository:

    deb http://mirrors.xbmc.org/apt/steamos alchemist main

Download the apt key

    wget -O - http://mirrors.xbmc.org/apt/steamos/steam@xbmc.org.gpg.key | sudo apt-key add


Create `/etc/apt/preferences`

    Code:
    Package: *
    Pin: origin mirrors.xbmc.org
    Pin-Priority: 500

    Package: *
    Pin: release l=SteamOS
    Pin-Priority: 900

Then do an update, and install xbmc

    sudo apt-get update
    sudo apt-get install xbmc

Then in Steam do "Add a non-steam shortcut" from the Library view, and add XBMC. Note that by default XBMC will not support a controller, so you need to have a keyboard or mouse plugged in so you can enable controller support in the XBMC settings.

After you enable the controller it will work without any other configuration.

References:

- http://forum.xbmc.org/showthread.php?tid=197422&pid=1730721#pid1730721
- http://steamcommunity.com/groups/steamuniverse/discussions/1/648816742742587380/
- http://www.reddit.com/r/linux/comments/1sw978/xbmc_steamos/