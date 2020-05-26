# Customizing AAs

### What are Alternate Advancements?

When a player reaches level 51, they unlock the option to dedicate experience they gain to be sent to Alternate Advancements. AAs are accessed inside Everquest using the default "v" hotkey. Due to the general nature of how AA's work, the Database Schemas that represent them on the server can be slightly complex to understand.

### Legend

AA's are grouped together by ranks. For example, Innate Runspeed has many ranks to represent the levels it can be trained. Each rank has a unique id assigned to it.

### Tools

[The PEQ PHP Editor](https://github.com/ProjectEQ/peqphpeditor) is the only tool to support editing AAs without directly accessing the database.

### Commands

* **\#reloadaa** - If you change any AA data in the database, you can use this command to reload it.
* **\#resetaa** - Target a player, it will reset all their spent AA's, refunding them the used points
* **\#resetaa\_timer** - Reset all AA timers for a player
* **\#setaapts \[value\]** - Set your or your player target's available AA points
* **\#setaaxp \[value\]** - Set your or your player target's AA experience

