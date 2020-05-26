---
description: >-
  This page lists the commands that are available in-game, based on assigned
  Account Status, for your EQEmu Server.
---

# Commands Reference

Often referred to as "GM Commands", the following commands can be allowed based on the player's Account Status.

| Command | Description |
| :--- | :--- |
| \#acceptrules | \[acceptrules\] - Accept the EQEmu Agreement |
| \#advnpcspawn | \[maketype\|makegroup\|addgroupentry\|addgroupspawn\]\[removegroupspawn\|movespawn\|editgroupbox\|cleargroupbox\] |
| \#aggro | \(range\) \[-v\] - Display aggro information for all mobs 'range' distance from your target. -v is verbose faction info. |
| \#aggrozone | \[aggro\] - Aggro every mob in the zone with X aggro. Default is 0. Not recommend if you are not invulnerable. |
| \#ai | \[factionid/spellslist/con/guard/roambox/stop/start\] - Modify AI on NPC target |
| \#altactivate | \[argument\] - activates alternate advancement abilities, use altactivate help for more information |
| \#appearance | \[type\] \[value\] - Send an appearance packet for you or your target |
| \#attack | \[targetname\] - Make your NPC target attack targetname |
| \#ban | \[name\] - Ban by character name |
| \#bestz | Ask map for a good Z coord for your x,y coords. |
| \#bind | Sets your targets bind spot to their current location |
| \#bot | Type "\#bot help" to the see the list of available commands for bots. |
| \#bugtrack | \[bug description\] - Report a bug |
| \#cast | \[spellid\] - Cast a spell |
| \#castspell | \[spellid\] - Cast a spell |
| \#charbackup | \[list/restore\] - Query or restore character backups |
| \#chat | \[channel num\] \[message\] - Send a channel message to all zones |
| \#checklos | Check for line of sight to your target |
| \#clearquestitems | Clears quest items for multiquesting currently on the target npc. |
| \#connectworld | Make zone attempt to connect to worldserver |
| \#connectworldserver | Make zone attempt to connect to worldserver |
| \#copychar | \[character name\] \[new character\] \[new account id\] - Create a copy of a character |
| \#corpse | Manipulate corpses, use with no arguments for help |
| \#crashtest | Crash the zoneserver |
| \#cvs | Summary of client versions currently online. |
| \#d1 | \[type\] \[spell\] \[damage\] - Send an OP\_Action packet with the specified values |
| \#damage | \[amount\] - Damage your target |
| \#datarate | \[rate\] - Query/set datarate |
| \#date | \[yyyy\] \[mm\] \[dd\] \[HH\] \[MM\] - Set EQ time |
| \#dbspawn | \[npctypeid\] \[factionid\] - Spawn an NPC from the db |
| \#dbspawn2 | \[spawngroup\] \[respawn\] \[variance\] - Spawn an NPC from a predefined row in the spawn2 table |
| \#delacct | \[accountname\] - Delete an account |
| \#deletegraveyard | \[zone name\] - Deletes the graveyard for the specified zone. |
| \#depop | Depop your NPC target |
| \#depopzone | Depop the zone |
| \#disablerecipe | \[recipe id\] - Disabled the specified recipe ID. |
| \#distance | Reports the distance between you and your target. |
| \#doanim | \[animnum\] \[type\] - Send an EmoteAnim for you or your target |
| \#emote | \['name'/'world'/'zone'\] \[type\] \[message\] - Send an emote message |
| \#emotesearch | Searches loaded NPC emotes |
| \#emoteview | Lists all of a NPCs loaded emotes |
| \#enablerecipe | \[recipe id\] - Enables the specified recipe ID. |
| \#equipitem | \[slotid\(0-21\)\] - Equip the item on your cursor into the specified slot |
| \#face | \[number of face\] - Sets you or your target's face to face number, temporarily. |
| \#fear | View and edit fear grids and hints |
| \#finditem | Finds an item by name or ID. |
| \#findnpctype | \[search criteria\] - Search database NPC types |
| \#findspell | \[searchstring\] - Search for a spell |
| \#findzone | \[search criteria\] - Search database for zone |
| \#fixmob | \[nextrace\|prevrace\|gender\|nexttexture\|prevtexture\|nexthelm\|prevhelm\] - Manipulate appearance of your NPC target |
| \#flag | \[status\] \[acctname\] - Refresh your admin status, or set an account's admin status if arguments provided |
| \#flagedit | Edit zone flags on your target |
| \#flags | Displays the flags of you or your target |
| \#flymode | \[0/1/2\] - Set your or your player target's flymode to off/on/levitate |
| \#fov | Check wether you're behind or in your target's field of view |
| \#freeze | Freeze your target |
| \#fz | \[search criteria\] - Search database for zone |
| \#gassign | \[id\] - Assign targetted NPC to predefined wandering grid id |
| \#gender | \[0/1/2\] - Change your or your target's gender to male/female/neuter |
| \#getplayerburriedcorp | Get the target's total number of burried player corpses. |
| \#getvariable | \[varname\] - Get the value of a variable from the database |
| \#gi | \[itemid\] - Gives your target an item. |
| \#ginfo | Get group info on target. |
| \#giveitem | \[itemid\] \[charges\] - Summon an item onto your target's cursor. Charges are optional. |
| \#givemoney | \[pp\] \[gp\] \[sp\] \[cp\] - Gives specified amount of money to the target player. |
| \#globalview | Lists all qglobals in cache if you were to do a quest with this target. |
| \#gm | Turn player target's or your GM flag on or off |
| \#gmhideme | Hides you from /who and /who all and makes you invisible to players. |
| \#gmspeed | \[on/off\] - Turn GM speed hack on/off for you or your player target |
| \#goto | \[x\] \[y\] \[z\] - Teleport to the provided coordinates or to your target |
| \#grid | \[add/delete\] \[grid\_num\] \[wandertype\] \[pausetype\] - Create/delete a wandering grid |
| \#guild help | Guild manipulation commands. Use argument help for more info. |
| \#guildapprove | \[guildapproveid\] - Approve a guild with specified ID \(guild creator receives the id\) |
| \#guildcreate | \[guildname\] - Creates an approval setup for guild name specified |
| \#guildlist | \[guildapproveid\] - Lists character names who have approved the guild specified by the approve id |
| \#haste | \[percentage\] - Set your haste percentage |
| \#hatelist | Display hate list for target. |
| \#heal | Completely heal your target |
| \#help | \[search term\] - List available commands and their description, specify partial command as argument to search |
| \#hideme | \[on/off\] - Hide yourself from spawn lists. |
| \#hp | Refresh your HP bar from the server. |
| \#incstat | Increases or Decreases a client's stats permanently. |
| \#instance | Modify Instances |
| \#interrogateinv | use \[help\] argument for available options |
| \#interrupt | \[message id\] \[color\] - Interrupt your casting. Arguments are optional. |
| \#invul | \[on/off\] - Turn player target's or your invulnerable flag on or off |
| \#invulnerable | \[on/off\] - Turn player target's or your invulnerable flag on or off |
| \#ipban | \[IP address\] - Ban IP by character name |
| \#ipc | Toggle an NPC's interactive flag |
| \#iplookup | \[charname\] - Look up IP address of charname |
| \#iteminfo | Get information about the item on your cursor |
| \#itemsearch | \[search criteria\] - Search for an item |
| \#kick | \[charname\] - Disconnect charname |
| \#kill | Kill your target |
| \#lastname | \[new lastname\] - Set your or your player target's lastname |
| \#level | \[level\] - Set your or your target's level |
| \#listnpcs | \[name/range\] - Search NPCs |
| \#loc | Print out your or your target's current location and heading |
| \#lock | Lock the worldserver |
| \#log | Search character event log |
| \#logs | \[status |
| \#logsql | Enable SQL logging |
| \#los | \[on/off\] - Tells you if you have line of sight to your target. |
| \#makepet | \[level\] \[class\] \[race\] \[texture\] - Make a pet |
| \#mana | Fill your or your target's mana |
| \#manaburn | Use AA Wizard class skill manaburn on target |
| \#manastat | Report your or your target's cur/max mana |
| \#memspell | \[slotid\] \[spellid\] - Memorize spellid in the specified slot |
| \#mlog | Manage log settings |
| \#modifynpcstat | Modifys a NPC's stats |
| \#motd | \[new motd\] - Set message of the day |
| \#movechar | \[charname\] \[zonename\] - Move charname to zonename |
| \#mysql | Mysql CLI, see 'help' for options. |
| \#mystats | Show details about you or your pet. |
| \#name | \[newname\] - Rename your player target |
| \#nologs | \[status |
| \#npccast | \[targetname/entityid\] \[spellid\] - Causes NPC target to cast spellid on targetname/entityid |
| \#npcedit | \[column\] \[value\] - Mega NPC editing command |
| \#npcemote | \[message\] - Make your NPC target emote a message. |
| \#npcloot | \[show/money/add/remove\] \[itemid/all/money: pp gp sp cp\] - Manipulate the loot an NPC is carrying |
| \#npcsay | \[message\] - Make your NPC target say a message. |
| \#npcshout | \[message\] - Make your NPC target shout a message. |
| \#npcspawn | \[create/add/update/remove/delete\] - Manipulate spawn DB |
| \#npcspecialatk | \[flagchar\] \[perm\] - Set NPC special attack flags. Flags are E\(nrage\) F\(lurry\) R\(ampage\) S\(ummon\). |
| \#npcspecialattack | \[flagchar\] \[perm\] - Set NPC special attack flags. Flags are E\(nrage\) F\(lurry\) R\(ampage\) S\(ummon\). |
| \#npcspecialattk | \[flagchar\] \[perm\] - Set NPC special attack flags. Flags are E\(nrage\) F\(lurry\) R\(ampage\) S\(ummon\). |
| \#npcstats | Show stats about target NPC |
| \#npctypespawn | \[npctypeid\] \[factionid\] - Spawn an NPC from the db |
| \#nukebuffs | Strip all buffs on you or your target |
| \#nukeitem | \[itemid\] - Remove itemid from your player target's inventory |
| \#object | List\|Add\|Edit\|Move\|Rotate\|Copy\|Save\|Undo\|Delete - Manipulate static and tradeskill objects within the zone |
| \#oocmute | \[1/0\] - Mutes OOC chat |
| \#path | View and edit pathing |
| \#peekinv | \[worn/cursor/inv/bank/trade/all\] - Print out contents of your player target's inventory |
| \#peqzone | \[zonename\] - Go to specified zone, if you have &gt; 75% health |
| \#permaclass | \[classnum\] - Change your or your player target's class \(target is disconnected\) |
| \#permagender | \[gendernum\] - Change your or your player target's gender \(zone to take effect\) |
| \#permarace | \[racenum\] - Change your or your player target's race \(zone to take effect\) |
| \#peval | \(expression\) - execute some perl |
| \#pf | Useless information. |
| \#picklock | Used to pick locks. |
| \#plugin | \(sub\) \[args\] - execute a plugin |
| \#printquestitems | Returns available quest items for multiquesting currently on the target npc. |
| \#profiledump | Dump profiling info to logs |
| \#profilereset | Reset profiling info |
| \#pvp | \[on/off\] - Set your or your player target's PVP status |
| \#qglobal | \[on/off/view\] - Toggles qglobal functionality on an NPC |
| \#qtest | QueryServ testing command. |
| \#race | \[racenum\] - Change you or your target's race. Use \#race 0 to return to normal. This is temporary, you revert back to normal upon zoning. |
| \#raidloot | LEADER |
| \#randomfeatures | Randomly changes the Facial Features of your target |
| \#refreshgroup | Refreshes Group. |
| \#refundaa | Refunds your target's AA points, will disconnect them in the process as well. |
| \#reloademote | Reloads NPC emotes |
| \#reloadpl | Reloads quest scripts. -- Doesn't work with Lua! |
| \#reloadqst | Reloads quest scripts. -- Doesn't work with Lua! |
| \#reloadquest | Clear quest cache |
| \#reloadstatic | Reload Static Zone Data |
| \#reloadworld | Reloads all scripts and repops all NPC's globally. |
| \#reloadzonepoints | Reload zone points from database |
| \#reloadzps | Reload zone points from database |
| \#repop | Repop the zone with optional delay. Using \#repop force forcefully resets spawn timers. |
| \#resetaa | Resets a Player's AA in their profile. |
| \#revoke | \[charname\] \[1/0\] - Makes charname unable to talk on OOC and unable to use /tell. |
| \#rules | \(subcommand\) - Manage server rules |
| \#save | Force your player or player corpse target to be saved to the database |
| \#scribespell | \[spellid\] - Scribe specified spell in your target's spell book. |
| \#scribespells | \[maxlevel\], \[minlevel\] - Scribe all spells for you or your player target that are usable by them, up to level specified. |
| \#search | Finds an item by name or ID. |
| \#sendzonespawns | Refresh spawn list for all clients in zone |
| \#serverinfo | Get OS info about server host |
| \#serverrules | Read this server's rules |
| \#serversidename | Prints target's server side name |
| \#setaaexp | \[amount\] - Adds the amount of AA experience you specified to you or your target. |
| \#setaapoints | \[AA\|group\|raid\] \[new AA points value\] - Increase your AA points based on amount specified. |
| \#setaapts | \[value\] - Set your or your player target's available AA points |
| \#setaaxp | \[value\] - Set your or your player target's AA experience |
| \#setadventurepoints | Set you or your player target's available adventure points |
| \#setallskill | \[amount\] - Sets all your skills to any amount, from 0 to 400. |
| \#setanim | \[animnum\] - Set target's appearance to animnum |
| \#setcrystals | Set your or your player targets available radiant or ebon crystals |
| \#setexp | \[amount\] - Adds the amount of experience you specified to you or your target. |
| \#setfaction | \[faction number\] - Sets targeted NPC's faction in the database |
| \#setgraveyard | \[zone name\] - Creates a graveyard for the specified zone based on your target's LOC. |
| \#setitemstatus | \[itemid\] \[status\] - Set the minimum admin status required to use itemid |
| \#setlanguage | \[language ID\] \[value\] - Set your target's language skillnum to value |
| \#setlsinfo | \[email\] \[password\] - Set login server email address and password. |
| \#setpass | \[accountname\] \[password\] - Set local password for accountname |
| \#setpvppoints | Set your or your player targets PVP points |
| \#setskill | \[skillnum\] \[value\] - Set your target's skill skillnum to value |
| \#setskillall | \[value\] - Set all of your target's skills to value |
| \#setstartzone | \[zoneid\] - Set target's starting zone. Set to zero to allow the player to use /setstartcity |
| \#setstat | Sets the stats to a specific value. |
| \#setxp | \[value\] - Set your or your player target's experience |
| \#showbuffs | List buffs active on your target or you if no target |
| \#showpetspell | \[spellid/searchstring\] - search pet summoning spells |
| \#showskills | Show the values of your or your player target's skills |
| \#showstats | Show details about you or your target |
| \#shutdown | Shut this zone process down |
| \#si | \[itemid\], \[charges\] - Spawns an item with the chosen charges. |
| \#size | \[size\] - Change size of you or your target |
| \#spawn | \[name\] \[race\] \[level\] \[material\] \[hp\] \[gender\] \[class\] \[priweapon\] \[secweapon\] \[merchantid\] - Spawn an NPC |
| \#spawnfix | Find targeted NPC in database based on its X/Y/heading and update the database to make it spawn at your current location/heading. |
| \#spawnstatus | Show respawn timer status |
| \#spellinfo | \[spellid\] - Get detailed info about a spell |
| \#spfind | \[searchstring\] - Search for a spell |
| \#stun | \[duration\] - Stuns you or your target for duration |
| \#summon | \[charname\] - Summons your player/npc/corpse target, or charname if specified |
| \#summonburriedplayerc | Summons the target's oldest burried corpse, if any exist. |
| \#summonitem | \[itemid\] \[charges\] - Summon an item onto your cursor. Charges are optional. |
| \#suspend | Suspend by character name and for specificed number of days |
| \#synctod | Send a time of day update to every client in zone |
| \#task | \(subcommand\) - Task system commands |
| \#testspawn | \[memloc\] \[value\] - spawns a NPC for you only, with the specified values set in the spawn struct |
| \#testspawnkill | Sends an OP\_Death packet for spawn made with \#testspawn |
| \#texture | \[texture\] \[helmtexture\] - Change your or your target's appearance, use 255 to show equipment |
| \#time | \[HH\] \[MM\] - Set EQ time |
| \#timers | Display persisten timers for target |
| \#timezone | \[HH\] \[MM\] - Set timezone. Minutes are optional |
| \#title | \[text\] - Set your or your player target's title |
| \#traindisc | \[level\] - Trains all the disciplines usable by the target, up to level specified. \(may freeze client for a few seconds\) |
| \#undyeme | Remove dye from all of your armor slots |
| \#unfreeze | Unfreeze your target |
| \#unlock | Unlock the worldserver |
| \#unscribespell | \[spellid\] - Unscribe specified spell from your target's spell book. |
| \#unscribespells | Clear out your or your player target's spell book. |
| \#uptime | \[zone server id\] - Get uptime of worldserver, or zone server if argument provided |
| \#version | Display current version of EQEmu server |
| \#viewmessage | \[id\] - View messages in your tell queue |
| \#viewmessages | \[id\] - View messages in your tell queue |
| \#viewnpctype | \[npctype id\] - Show info about an npctype |
| \#viewpetition | \[petition number\] - View a petition |
| \#wc | \[wear slot\] \[material\] - Sends an OP\_WearChange for your target |
| \#weather | \[0/1/2/3\] \(Off/Rain/Snow/Manual\) - Change the weather |
| \#worldshutdown | Shut down world and all zones |
| \#wp | \[add/delete\] \[grid\_num\] \[pause\] \[wp\_num\] - Add/delete a waypoint to/from a wandering grid |
| \#wpadd | \[pause\] - Add your current location as a waypoint to your NPC targets AI path |
| \#wpinfo | Show waypoint info about your NPC target |
| \#xtargets | Show your targets Extended Targets and optionally set how many xtargets they can have |
| \#zclip | \[min\] \[max\] - modifies and resends zhdr packet |
| \#zcolor | \[red\] \[green\] \[blue\] - Change sky color |
| \#zhdr | \[zonename\] - Load zheader for zonename from the database |
| \#zheader | \[zonename\] - Load zheader for zonename from the database |
| \#zone | \[zonename\] \[x\] \[y\] \[z\] - Go to specified zone \(co-ordinates optional\) |
| \#zonebootup | \[ZoneServerID\] \[shortname\] - Make a zone server boot a specific zone |
| \#zoneinstance | \[instanceid\] \[x\] \[y\] \[z\] - Go to specified instance zone \(co-ordinates optional\) |
| \#zonelock | \[list/lock/unlock\] - Set/query lock flag for zoneservers |
| \#zoneshutdown | \[shortname\] - Shut down a zone server |
| \#zonestatus | Show connected zoneservers, synonymous with /servers |
| \#zsafecoords | \[x\] \[y\] \[z\] - Set safe co-ordinates |
| \#zsave | Saves zheader to the database |
| \#zsky | \[skytype\] - Change zone sky type |
| \#zstats | Show info about zone header |
| \#zunderworld | \[zcoord\] - Sets the underworld using zcoord |
| \#zuwcoords | \[z coord\] - Set underworld coord |

