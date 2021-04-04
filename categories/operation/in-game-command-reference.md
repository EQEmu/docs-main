---
description: >-
  This page lists the commands that are available in-game, based on assigned
  Account Status, for your EQEmu Server.
---

# Commands Reference

Often referred to as "GM Commands", the following commands can be allowed based on the player's Account Status.

| Command | Description |
| :--- | :--- |

| \#acceptrules | \[acceptrules\] Accept the EQEmu Agreement |
| \#advnpcspawn | \[maketype\|makegroup\|addgroupentry\|addgroupspawn\]\[removegroupspawn\|movespawn\|editgroupbox\|cleargroupbox\] |
| \#aggro | \(range\) \[-v\] Display aggro information for all mobs 'range' distance from your target. -v is verbose faction info. |
| \#aggrozone | \[aggro\] Aggro every mob in the zone with X aggro. Default is 0. Not recommend if you're not invulnerable. |
| \#ai | \[factionid/spellslist/con/guard/roambox/stop/start\] Modify AI on NPC target |
| \#appearance | \[type\] \[value\] Send an appearance packet for you or your target |
| \#apply_shared_memory | \[shared_memory_name\] Tells every zone and world to apply a specific shared memory segment by name. |
| \#attack | \[targetname\] Make your NPC target attack targetname |
| \#augmentitem | Force augments an item. Must have the augment item window open. |
| \#ban | \[name\] \[reason\]- Ban by character name |
| \#beard | Change the beard of your target |
| \#beardcolor | Change the beard color of your target |
| \#bestz | Ask map for a good Z coord for your x,y coords. |
| \#bind | Sets your targets bind spot to their current location |
| \#bot | Type \"| \#bot help\" or \"^help\" to the see the list of available commands for bots. |
| \#camerashake | Shakes the camera on everyone's screen globally. |
| \#castspell | \[spellid\] Cast a spell |
| \#chat | \[channel num\] \[message\] Send a channel message to all zones |
| \#checklos | Check for line of sight to your target |
| \#copycharacter | \[source_char_name\] \[dest_char_name\] \[dest_account_name\] Copies character to destination account |
| \#corpse | Manipulate corpses, use with no arguments for help |
| \#corpsefix | Attempts to bring corpses from underneath the ground within close proximity of the player |
| \#crashtest | Crash the zoneserver |
| \#cvs | Summary of client versions currently online. |
| \#damage | \[amount\] Damage your target |
| \#databuckets | View\|Delete \[key\] \[limit\]- View data buckets, limit 50 default or Delete databucket by key |
| \#date | \[yyyy\] \[mm\] \[dd\] \[HH\] \[MM\] Set EQ time |
| \#dbspawn2 | \[spawngroup\] \[respawn\] \[variance\] Spawn an NPC from a predefined row in the spawn2 table |
| \#delacct | \[accountname\] Delete an account |
| \#deletegraveyard | \[zone name\] Deletes the graveyard for the specified zone. |
| \#delpetition | \[petition number\] Delete a petition |
| \#depop | Depop your NPC target |
| \#depopzone | Depop the zone |
| \#details | Change the details of your target \(Drakkin Only\) |
| \#devtools | Manages devtools |
| \#disablerecipe | \[recipe_id\] Disables a recipe using the recipe id. |
| \#disarmtrap | Analog for ldon disarm trap for the newer clients since we still don't have it working. |
| \#distance | Reports the distance between you and your target. |
| \#doanim | \[animnum\] \[type\] Send an EmoteAnim for you or your target |
| \#dz | Manage expeditions and dynamic zone instances |
| \#dzkickplayers | Removes all players from current expedition. \(/kick players alternative for pre-RoF clients\) |
| \#editmassrespawn | \[name-search\] \[second-value\] Mass \(Zone wide\) NPC respawn timer editing command |
| \#emote | \['name'/'world'/'zone'\] \[type\] \[message\] Send an emote message |
| \#emotesearch | Searches NPC Emotes |
| \#emoteview | Lists all NPC Emotes |
| \#enablerecipe | \[recipe_id\] Enables a recipe using the recipe id. |
| \#endurance | Restores you or your target's endurance. |
| \#equipitem | \[slotid\(0-21\)\] Equip the item on your cursor into the specified slot |
| \#face | Change the face of your target |
| \#faction | \[Find \(criteria | all \) | Review \(criteria | all\) | Reset \(id\)\] Resets Player's Faction |
| \#findaliases | \[search criteria\]- Searches for available command aliases, by alias or command |
| \#findnpctype | \[search criteria\] Search database NPC types |
| \#findrace | \[search criteria\] Search for a race |
| \#findspell | \[search criteria\] Search for a spell |
| \#findzone | \[search criteria\] Search database zones |
| \#fixmob | \[race\|gender\|texture\|helm\|face\|hair\|haircolor\|beard\|beardcolor\|heritage\|tattoo\|detail\] \[next\|prev\] Manipulate appearance of your target |
| \#flag | \[status\] \[acctname\] Refresh your admin status, or set an account's admin status if arguments provided |
| \#flagedit | Edit zone flags on your target |
| \#flags | displays the flags of you or your target |
| \#flymode | \[0/1/2/3/4/5\] Set your or your player target's flymode to ground/flying/levitate/water/floating/levitate_running |
| \#fov | Check whether you are behind or in your target's field of view |
| \#freeze | Freeze your target |
| \#gassign | \[id\] Assign targeted NPC to predefined wandering grid id |
| \#gearup | Developer tool to quickly equip a character |
| \#gender | \[0/1/2\] Change your or your target's gender to male/female/neuter |
| \#getplayerburiedcorpsecount | Get the target's total number of buried player corpses. |
| \#getvariable | \[varname\] Get the value of a variable from the database |
| \#ginfo | get group info on target. |
| \#giveitem | \[itemid\] \[charges\] Summon an item onto your target's cursor. Charges are optional. |
| \#givemoney | \[pp\] \[gp\] \[sp\] \[cp\] Gives specified amount of money to the target player. |
| \#globalview | Lists all qglobals in cache if you were to do a quest with this target. |
| \#gm | Turn player target's or your GM flag on or off |
| \#gmspeed | \[on/off\] Turn GM speed hack on/off for you or your player target |
| \#gmzone | \[zone_short_name\] \[zone_version=0\] \[identifier=gmzone\] Zones to a private GM instance |
| \#goto | \[playername\] or \[x y z\] \[h\] Teleport to the provided coordinates or to your target |
| \#grid | \[add/delete\] \[grid_num\] \[wandertype\] \[pausetype\] Create/delete a wandering grid |
| \#guild | Guild manipulation commands. Use argument help for more info. |
| \#guildapprove | \[guildapproveid\] Approve a guild with specified ID \(guild creator receives the id\) |
| \#guildcreate | \[guildname\] Creates an approval setup for guild name specified |
| \#guildlist | \[guildapproveid\] Lists character names who have approved the guild specified by the approve id |
| \#hair | Change the hair style of your target |
| \#haircolor | Change the hair color of your target |
| \#haste | \[percentage\] Set your haste percentage |
| \#hatelist |  Display hate list for target. |
| \#heal | Completely heal your target |
| \#helm | Change the helm of your target |
| \#help | \[search term\] List available commands and their description, specify partial command as argument to search |
| \#heritage | Change the heritage of your target \(Drakkin Only\) |
| \#heromodel | \[hero model\] \[slot\] Full set of Hero's Forge Armor appearance. If slot is set, sends exact model just to slot. |
| \#hideme | \[on/off\] Hide yourself from spawn lists. |
| \#hotfix | \[hotfix_name\] Reloads shared memory into a hotfix, equiv to load_shared_memory followed by apply_shared_memory |
| \#hp | Refresh your HP bar from the server. |
| \#incstat | Increases or Decreases a client's stats permanently. |
| \#instance | Modify Instances |
| \#interrogateinv | use \[help\] argument for available options |
| \#interrupt | \[message id\] \[color\] Interrupt your casting. Arguments are optional. |
| \#invsnapshot | Manipulates inventory snapshots for your current target |
| \#invul | \[on/off\] Turn player targets or your invulnerable flag on or off |
| \#ipban | \[IP address\] Ban IP by character name |
| \#iplookup | \[charname\] Look up IP address of charname |
| \#iteminfo | Get information about the item on your cursor |
| \#itemsearch | \[search criteria\] Search for an item |
| \#kick | \[charname\] Disconnect charname |
| \#kill | Kill your target |
| \#killallnpcs |  \[npc_name\] Kills all npcs by search name, leave blank for all attackable NPC's |
| \#lastname | \[new lastname\] Set your or your player target's lastname |
| \#level | \[level\] Set your or your target's level |
| \#list | \[npcs\|players\|corpses\|doors\|objects\] \[search\] Search entities |
| \#listnpcs | \[name/range\] Search NPCs |
| \#listpetition | List petitions |
| \#load_shared_memory | \[shared_memory_name\] Reloads shared memory and uses the input as output |
| \#loc | Print out your or your target's current location and heading |
| \#lock | Lock the worldserver |
| \#logs | Manage anything to do with logs |
| \#logtest | Performs log performance testing. |
| \#makepet | \[level\] \[class\] \[race\] \[texture\] Make a pet |
| \#mana | Fill your or your target's mana |
| \#maxskills | Maxes skills for you. |
| \#memspell | \[slotid\] \[spellid\] Memorize spellid in the specified slot |
| \#merchant_close_shop | Closes a merchant shop |
| \#merchant_open_shop | Opens a merchant’s shop |
| \#modifynpcstat | Modifys a NPC's stats |
| \#motd | \[new motd\] Set message of the day |
| \#movechar | \[charname\] \[zonename\] Move charname to zonename |
| \#movement | Various movement commands |
| \#myskills | Show details about your current skill levels |
| \#mysql | Mysql CLI, see 'help' for options. |
| \#mysqltest | Akkadius MySQL Bench Test |
| \#mystats | Show details about you or your pet |
| \#name | \[newname\] Rename your player target |
| \#netstats | Gets the network stats for a stream. |
| \#network | Admin commands for the udp network interface. |
| \#npccast | \[targetname/entityid\] \[spellid\] Causes NPC target to cast spellid on targetname/entityid |
| \#npcedit | \[column\] \[value\] Mega NPC editing command |
| \#npceditmass | \[name-search\] \[column\] \[value\] Mass \(Zone wide\) NPC data editing command |
| \#npcemote | \[message\] Make your NPC target emote a message. |
| \#npcloot | \[show/money/add/remove\] \[itemid/all/money: pp gp sp cp\] Manipulate the loot an NPC is carrying |
| \#npcsay | \[message\] Make your NPC target say a message. |
| \#npcshout | \[message\] Make your NPC target shout a message. |
| \#npcspawn | \[create/add/update/remove/delete\] Manipulate spawn DB |
| \#npcspecialattk | \[flagchar\] \[perm\] Set NPC special attack flags. Flags are E\(nrage\) F\(lurry\) R\(ampage\) S\(ummon\). |
| \#npcstats | Show stats about target NPC |
| \#npctype_cache | \[id\] or all Clears the npc type cache for either the id or all npcs. |
| \#npctypespawn | \[npctypeid\] \[factionid\] Spawn an NPC from the db |
| \#nudge | Nudge your target's current position by specific values |
| \#nukebuffs | Strip all buffs on you or your target |
| \#nukeitem | \[itemid\] Remove itemid from your player target's inventory |
| \#object | List\|Add\|Edit\|Move\|Rotate\|Copy\|Save\|Undo\|Delete Manipulate static and tradeskill objects within the zone |
| \#oocmute | \[1/0\] Mutes OOC chat |
| \#opcode | opcode management |
| \#packetprofile | Dump packet profile for target or self. |
| \#path | view and edit pathing |
| \#peekinv | \[equip/gen/cursor/poss/limbo/curlim/trib/bank/shbank/allbank/trade/world/all\] Print out contents of your player target's inventory |
| \#peqzone | \[zonename\] Go to specified zone if you have > 75% health |
| \#permaclass | \[classnum\] Change your or your player target's class \(target is disconnected\) |
| \#permagender | \[gendernum\] Change your or your player target's gender \(zone to take effect\) |
| \#permarace | \[racenum\] Change your or your player target's race \(zone to take effect\) |
| \#petitioninfo | \[petition number\] Get info about a petition |
| \#petname | \[newname\] Temporarily renames your pet. Leave name blank to restore the original name. |
| \#pf | Display additional mob coordinate and wandering data |
| \#picklock | Analog for ldon pick lock for the newer clients since we still don't have it working. |
| \#profanity | Manage censored language. |
| \#profiledump | Dump profiling info to logs |
| \#profilereset | Reset profiling info |
| \#proximity | Shows NPC proximity |
| \#push | Lets you do spell push |
| \#pvp | \[on/off\] Set your or your player target's PVP status |
| \#qglobal | \[on/off/view\] Toggles qglobal functionality on an NPC |
| \#questerrors | Shows quest errors. |
| \#race | \[racenum\] Change your or your target's race. Use racenum 0 to return to normal |
| \#raidloot | LEADER\|GROUPLEADER\|SELECTED\|ALL Sets your raid loot settings if you have permission to do so. |
| \#randomfeatures | Temporarily randomizes the Facial Features of your target |
| \#refreshgroup | Refreshes Group. |
| \#reloadaa | Reloads AA data |
| \#reloadallrules | Executes a reload of all rules. |
| \#reloademote | Reloads NPC Emotes |
| \#reloadlevelmods", nullptr, 255, command_reloadlevelmods\) \|\|
| \#reloadmerchants", nullptr, 255, command_reloadmerchants\) \|\|
| \#reloadperlexportsettings", nullptr, 255, command_reloadperlexportsettings\) \|\|
| \#reloadqst | Clear quest cache \(any argument causes it to also stop all timers\) |
| \#reloadrulesworld | Executes a reload of all rules in world specifically. |
| \#reloadstatic | Reload Static Zone Data |
| \#reloadtitles | Reload player titles from the database |
| \#reloadtraps | Repops all traps in the current zone. |
| \#reloadworld | \[0\|1\] Clear quest cache \(0 no repop, 1 repop\) |
| \#reloadzps | Reload zone points from database |
| \#repop | \[delay\] Repop the zone with optional delay |
| \#resetaa | Resets a Player's AA in their profile and refunds spent AA's to unspent, may disconnect player. |
| \#resetaa_timer | Command to reset AA cooldown timers. |
| \#revoke | \[charname\] \[1/0\] Makes charname unable to talk on OOC |
| \#roambox | Manages roambox settings for an NPC |
| \#rules | \(subcommand\) Manage server rules |
| \#save | Force your player or player corpse target to be saved to the database |
| \#scale | Handles npc scaling |
| \#scribespell | \[spellid\] Scribe specified spell in your target's spell book. |
| \#scribespells | \[max level\] \[min level\] Scribe all spells for you or your player target that are usable by them, up to level specified. \(may freeze client for a few seconds\) |
| \#sendzonespawns | Refresh spawn list for all clients in zone |
| \#sensetrap | Analog for ldon sense trap for the newer clients since we still don't have it working. |
| \#serverinfo | Get OS info about server host |
| \#serverrules | Read this server's rules |
| \#setaapts | \[value\] Set your or your player target's available AA points |
| \#setaaxp | \[value\] Set your or your player target's AA experience |
| \#setadventurepoints | Set your or your player target's available adventure points |
| \#setanim | \[animnum\] Set target's appearance to animnum |
| \#setcrystals | \[value\] Set your or your player target's available radiant or ebon crystals |
| \#setfaction | \[faction number\] Sets targeted NPC's faction in the database |
| \#setgraveyard | \[zone name\] Creates a graveyard for the specified zone based on your target's LOC. |
| \#setlanguage | \[language ID\] \[value\] Set your target's language skillnum to value |
| \#setlsinfo | \[email\] \[password\] Set login server email address and password \(if supported by login server\) |
| \#setpass | \[accountname\] \[password\] Set local password for accountname |
| \#setpvppoints | \[value\] Set your or your player target's PVP points |
| \#setskill | \[skillnum\] \[value\] Set your target's skill skillnum to value |
| \#setskillall | \[value\] Set all of your target's skills to value |
| \#setstartzone | \[zoneid\] Set target's starting zone. Set to zero to allow the player to use /setstartcity |
| \#setstat | Sets the stats to a specific value. |
| \#setxp | \[value\] Set your or your player target's experience |
| \#showbonusstats | \[item\|spell\|all\] Shows bonus stats for target from items or spells. Shows both by default. |
| \#showbuffs | List buffs active on your target or you if no target |
| \#shownpcgloballoot | Show GlobalLoot entires on this npc |
| \#shownumhits | Shows buffs numhits for yourself. |
| \#showskills | Show the values of your or your player target's skills |
| \#showspellslist | Shows spell list of targeted NPC |
| \#showstats | Show details about you or your target |
| \#showzonegloballoot | Show GlobalLoot entires on this zone |
| \#showzonepoints | Show zone points for current zone |
| \#shutdown | Shut this zone process down |
| \#size | \[size\] Change size of you or your target |
| \#spawn | \[name\] \[race\] \[level\] \[material\] \[hp\] \[gender\] \[class\] \[priweapon\] \[secweapon\] \[merchantid\] Spawn an NPC |
| \#spawneditmass | Mass editing spawn command |
| \#spawnfix | Find targeted NPC in database based on its X/Y/heading and update the database to make it spawn at your current location/heading. |
| \#spawnstatus | Show respawn timer status |
| \#spellinfo | \[spellid\] Get detailed info about a spell |
| \#spoff | Sends OP_ManaChange |
| \#spon | Sends OP_MemorizeSpell |
| \#stun | \[duration\] Stuns you or your target for duration |
| \#summon | \[charname\] Summons your player/npc/corpse target, or charname if specified |
| \#summonburiedplayercorpse | Summons the target's oldest buried corpse, if any exist. |
| \#summonitem | \[itemid\] \[charges\] Summon an item onto your cursor. Charges are optional. |
| \#suspend | \[name\] \[days\] \[reason\] Suspend by character name and for specified number of days |
| \#task | \(subcommand\) Task system commands |
| \#tattoo | Change the tattoo of your target \(Drakkin Only\) |
| \#tempname | \[newname\] Temporarily renames your target. Leave name blank to restore the original name. |
| \#test | Test command |
| \#texture | \[texture\] \[helmtexture\] Change your or your target's appearance, use 255 to show equipment |
| \#time | \[HH\] \[MM\] Set EQ time |
| \#timers | Display persistent timers for target |
| \#timezone | \[HH\] \[MM\] Set timezone. Minutes are optional |
| \#title | \[text\] \[1 = create title table row\] Set your or your player target's title |
| \#titlesuffix | \[text\] \[1 = create title table row\] Set your or your player target's title suffix |
| \#traindisc | \[level\] Trains all the disciplines usable by the target, up to level specified. \(may freeze client for a few seconds\) |
| \#trapinfo | Gets information about the traps currently spawned in the zone. |
| \#tune | Calculate ideal statical values related to combat. |
| \#ucs | Attempts to reconnect to the UCS server |
| \#undyeme | Remove dye from all of your armor slots |
| \#unfreeze | Unfreeze your target |
| \#unlock | Unlock the worldserver |
| \#unscribespell | \[spellid\] Unscribe specified spell from your target's spell book. |
| \#unscribespells | Clear out your or your player target's spell book. |
| \#untraindisc | \[spellid\] Untrain specified discipline from your target. |
| \#untraindiscs | Untrains all disciplines from your target. |
| \#uptime | \[zone server id\] Get uptime of worldserver, or zone server if argument provided |
| \#version | Display current version of EQEmu server |
| \#viewnpctype | \[npctype id\] Show info about an npctype |
| \#viewpetition | \[petition number\] View a petition |
| \#wc | \[wear slot\] \[material\] Sends an OP_WearChange for your target |
| \#weather | \[0/1/2/3\] \(Off/Rain/Snow/Manual\) Change the weather |
| \#who | \[search\] |
| \#worldshutdown | Shut down world and all zones |
| \#worldwide | Performs world-wide GM functions such as cast \(can be extended for other commands\). Use caution |
| \#wp | \[add/delete\] \[grid_num\] \[pause\] \[wp_num\] \[-h\] Add/delete a waypoint to/from a wandering grid |
| \#wpadd | \[pause\] \[-h\] Add your current location as a waypoint to your NPC target's AI path |
| \#wpinfo | Show waypoint info about your NPC target |
| \#xtargets | Show your targets Extended Targets and optionally set how many xtargets they can have. |
| \#zclip | \[min\] \[max\] modifies and resends zhdr packet |
| \#zcolor | \[red\] \[green\] \[blue\] Change sky color |
| \#zheader | \[zonename\] Load zheader for zonename from the database |
| \#zone | \[zonename\] \[x\] \[y\] \[z\] Go to specified zone \(coords optional\) |
| \#zonebootup | \[ZoneServerID\] \[shortname\] Make a zone server boot a specific zone |
| \#zoneinstance | \[instanceid\] \[x\] \[y\] \[z\] Go to specified instance zone \(coords optional\) |
| \#zonelock | \[list/lock/unlock\] Set/query lock flag for zoneservers |
| \#zoneshutdown | \[shortname\] Shut down a zone server |
| \#zonespawn | Not implemented |
| \#zonestatus | Show connected zoneservers, synonymous with /servers |
| \#zopp | Troubleshooting command Sends a fake item packet to you. No server reference is created. |
| \#zsafecoords | \[x\] \[y\] \[z\] Set safe coords |
| \#zsave |  Saves zheader to the database |
| \#zsky | \[skytype\] Change zone sky type |
| \#zstats | Show info about zone header |
| \#zunderworld | \[zcoord\] Sets the underworld using zcoord |
| \#zuwcoords | \[z coord\] Set underworld coord |
