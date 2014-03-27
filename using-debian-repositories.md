# Using Debian Repositories
Default lines for `/etc/apt/sources.list`:

    ## internal SteamOS repo
    deb http://repo.steampowered.com/steamos alchemist main contrib non-free
    deb-src http://repo.steampowered.com/steamos alchemist main contrib non-free

To generate Debian Repositories, use [this site](http://debgen.simplylinux.ch/) and add those to that file. It should look something like this:

    deb http://ftp.us.debian.org/debian stable main



TODO: Integrate http://steamcommunity.com/groups/steamuniverse/discussions/1/648814396114274132/#p3