minecraft_tools
===============

Tools for managing Minecraft servers.

* api/rcon.py: A fully-featured RCON client API
* rcon_shell.py: An interactive console shell for the client API

Command-line options:

    $ python rcon_shell.py -h
    usage: rcon_shell.py [-h] [--host HOST] [--port PORT] --password PASSWORD
    
    Connect to a Minecraft RCON server
    
    optional arguments:
      -h, --help           show this help message and exit
      --host HOST          default: 127.0.0.1
      --port PORT          default: 25575
      --password PASSWORD  required

Sample usage:

    $ python rcon_shell.py --password xxxxxx
    Connecting to 127.0.0.1:25575...
      
      Welcome to the rcon shell. Enter commands here to send them
      to the RCON server. To quit, type "quit" or "q".
      
    rcon> say hello
    rcon> help 
    --- Showing help page 1 of 7 (/help <page>) ---
    /achievement give <stat_name> [player]
    /ban <name> [reason ...]
    /ban-ip <address|name> [reason ...]
    /banlist [ips|players]
    /clear <player> [item] [data]
    /debug <start|stop>
    /defaultgamemode <mode>
    rcon> quit
    Disconnected.

