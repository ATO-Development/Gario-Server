
# Gario Server
A funny and amazing agario Server


To install any plugins from the library, first do `plugin available` and remember the name of the plugin you want. then do `plugin install [name]` and you are set!

### How do I use other plugins

### How do I create a plugin? Is there Documentation

### Easy Verify
For those of you who have trouble with minions and such, this feature is for you. Currently, there is no program that can get through all of ogar unlimited's filterrs anddd features, but in some future, someone might be able to crack the other anti bot mesures. So we created easy verify, a currently foolproof system that filters out bots. To turn on, turn verify to 1 in config. Then when a player spawns, he is frozen at a spot and is given a 3 digit code. Then that player presses w to kill himself and types in the code in the nickname box. Afteword, when pressing play again, it shows a success message. Press w again to play.

### Minions
You use minions by doing `minion [yourid] [amount] [minionname]`. Then, they will start following your mouse. You can control those minions by useing E and R keys. E for split. R for feed. If that doesnt work because of you client, turn useER to 0 in config.ini. then in game, q key. If you press it, a B will appear next to your name. then controls will be normal except now ejecting and splitting will happen on your minions not you. you can reenter normal control mode by pressing q again. You can disable minions by doing `minion [id]` in console for just you or do `minion destroy` and it will remove all minions.

## Custom skins (guide)
You can use custom skins by putting them in customskins.txt
the format is `[shortcut] [skin]` for the skin field, to use a URL skin, you do `:http://url` DO NOT FORGET TO GET REID OF THE S IF IT IS HTTPS OR FORGET TO PUT A : BEFORE.To use an agario skin, use `%skinname`To use that skin in game simply do `<skinsshortuct>` and then your name

Currently, Gario listens on the following addresses and ports:
* *:88 - for the stats server (I would use it to track servers)
* *:443 - for the game server

~~(Once the game server is running, you can connect (locally) by typing `agar.io/?ip=127.0.0.1:443` into your browser's address bar.)~~ Now you should use our client !

## Custom Game modes
Gario has support for custom game modes. To switch between game modes, change the value of "serverGamemode" in the configurations file to the selected game mode id and restart the server. The current supported game modes are:

Id   | Name
-----|--------------
0    | Free For All
1    | Teams
2    | Experimental (As of 6/13/15)
3    | Timed FFA
4    | Virus Off (no virus's)
5    | UnlimitPVP - where you split can split indefinitly and rejoin instantly - 1v1 game (created by me)
6    | UnlimitFFA - same as above (unlimited pvp) except in ffa (created by me)
7    | Shrinking FFA, Shrinks the game as time passes
8    | Experimental v2
10   | Tournament
11   | Hunger Games
12   | Zombie Mode
13   | Team Z
14   | Team X
15   | NoCollision Teams
16   | NoCollision TeamZ
17   | NoCollision TeamX
18   | Leap - Where you leap instead of split, made by Ogarplus
20   | Rainbow FFA - Hint: Use with "setAcid(true)"
22   | BlackHole

## Console Commands
The current available console commands are listed here. Command names are not case sensitive, but player names are.
 
 - Help
   * Shows List Of Commands
 - Ophelp
   * Shows how to use OP
 - quickrestart
   * Quickly restart your server. This is not true restart and does not reduce memory;
 - multiverse [command] [arg]
   * manage multiple servers. see multiverse
 - Plugin [command]
   * manage plugins, reload, list, delete, add, available, install, update.
 - Chat [command] [args]
   * Chat from the console!. Commands: all, pm. For all `chat all [msg]` for pm `chat pm [id] [msg]`
 - Chatban [id]
   * Ban people from chatting!
 - Announce
   * Starts the high score announce feature
 - Verify [command] [id]
   * Verifies/reverifies a player .doing `verify reverify 1` forces 1 to verify again 
 - Minion [id] [amount] [minion names]
   * creates minions. to turn off, for a player do minion [id]. to destroy all minions do minion destroy
 - Update
   * gets current version of ogar unlimited and replaces the old with the new. Do update botnames to only update botnames or update skin to only update skins
 - Reset
   * Destroys everything and starts from scratch.
 - Range [start] [end] [command] [commandattr]
   * Does bulk commands. ex `range 1 10 freeze` would freeze players between 1 and 10
 - Pcmd [delay] [repeattime] [command] [commandat...]
   * Periodic commands
 - Opbyip [command] [ip]
   * Allows you to use the opbyip feature. the commands are add, remove, list, clear , record . This allows you to be automatically op based on your ip
 - Changelog [page]
   * Gets changelog from the servers
 - Explode [id]
   * explodes player
 - Blind [id]
   * Blinds/unblinds a player
 - Hide [id]
   * Hides/unhides a player
 - Split [ID] [Count]
   * Splits a player
 - Shrink [amount]
   * Shrinks the game (amount is optional)
 - Enlarge [amount]
   * Enlarges the game (amount is optional)
 - Freeze [id]
   * Freezes a player
 - Spawnmass [id] [mass]
   * sets a players spawnmass. set to 0 to return to normal value
 - Speed [id] [mass]
   * sets a players base speed. set to 0 to return to normal value
 - Colortext [color]
   * Changes console Color and Style (blue, green,red,yellow,bold,reset,dim,white, help)
 - Team [id] [team (r,g,b)]
   * Changes a players Team (you might have to split to see the changes though)
 - Resetvirus
   * Turns special viruses (from OP's) into normal ones
 - whitelist [IP]
   * whitelists an IP
 - Unwhitelist [IP]
   * Unwhitelists an IP
 - whitelist
   * Lists whitelist
 - Clearban
   * Clears ban list
 - Ban [IP]
   * Bans an IP and sends a MSG. Do ban record to record ban
 - Unban [IP]
   * Unbans an IP
 - Rainbow [id]
   * gives player rainbow effect
 - Kickbots [number]
   * Kicks a number of bots (leave field blank and it will kick all bots)
 - Killbots [number]
   * Kills a number of bots (leave field blank and it will kick all bots)
 - Restart [minutes]
   * Restarts the server after a number of minutes or if you leave min blank, restarts immediatly
 - Banlist
   * Lists banned IPs
 - Clearban
   * Clears ban list
 - Op [ID]
   * Makes player OP
 - Dop [ID]
   * De-OPs a player
 - Rop
   * Resets op
 - Pfmsg [delay] [duration] [x to repeat] [msg1] [msg2] [etc...]
   * Periodically sends a force message (seconds)
 - Spfmsg []
   * stops pfmsg
 - Pmsg [delay] [duration] [x to repeat] [msg1] [msg2] [etc...]
   * Periodically sends a message (seconds)
 - Spmsg []
   * stops pmsg
 - Troll [id]
   * You figure out this one, Its a suprise!
 - Fmsg [message 1] [message 2] [etc...]
   * Forces players to read a message, This is done by changeing leaderboard to msg, freezing players, and change their name temporarily
 - Msg [message1] [message2] [etc...]
   * Changes the leaderboard to a message for a short time
 - kick/killrange/ban [Start] [End]
   * Kicks/kills/bans in a range (eg: killrange 1 10 will kill players whos ids are between them)
 - Nojoin [id]
   * Makes person unable to join
 - Merge [id]
   * forces user to merge
 - Addbot [Number]
   * Adds [Number] of bots to the server. If an amount is not specified, 1 bot will be added.
 - Board [String 1] [String 2] [String 3] ...
   * Replaces the text on the leaderboard with the string text.
 - Boardreset
   * Resets the leaderboard to display the proper data for the current gamemode
 - Change [Config setting] [Value]
   * Changes a config setting to a value. Ex. "change serverMaxConnections 32" will change the variable serverMaxConnections to 32. Note that some config values (Like serverGamemode) are parsed before the server starts so changing them mid game will have no effect.
 - Clear
   * Clears the console output
 - Color [Player ID] [Red] [Green] [Blue]
   * Replaces the color of the specified player with this color.
 - Exit
   * Closes the server.
 - Food [X position] [Y position] [Mass]
   * Spawns a food cell at those coordinates. If a mass value is not specified, then the server will default to "foodStartMass" in the config.
 - Gamemode [Id]
   * Changes the gamemode of the server. Warning - This can cause problems.
 - Kick [Player ID]
   * Kicks the specified player or bot from the server.
 - Kill [Player ID]
   * Kills all cells belonging to the specified player.
 - Killall
   * Kills all player cells on the map.
 - Mass [Player ID] [Number]
   * Sets the mass of all cells belonging to the specified player to [Number].
 - Name [Player ID] [New Name]
   * Changes the name of the player with the specified id with [New Name].
 - Playerlist
   * Shows a list of connected players, their IP, player ID, the amount of cells they have, total mass, and their position.
 - Pause
   * Pauses/Unpauses the game.
 - Reload
   * Reloads the config file used by the server. However, the following values are not affected: serverPort, serverGamemode, serverBots, serverStatsPort, serverStatsUpdate.
 - Status
   * Shows the amount of players currently connected, time elapsed, memory usage (memory used/memory allocated), and the current gamemode.
 - Tp [Player ID] [X position] [Y position]
   * Teleports the specified player to the specified coordinates.
 - Virus [X position] [Y position] [Mass]
   * Spawns a virus cell at those coordinates. If a mass value is not specified, then the server will default to "virusStartMass" in the config.
