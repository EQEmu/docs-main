# NPC Aggro

Let's create a new faction. For this example, the NPCs on this faction will be KOS to all PCs except Erudites, whom they will con amiable. These NPCs will also attack other NPCs whom primary faction is Heretic. If anyone kills these NPCs, we will have them lose 10 points of faction with their faction \(the new one we're creating\) and gain 5 points with Heretic.

### Create the new base faction to faction\_list.

Create a new entry in faction\_list.  Since we want them to start out KOS to everyone except Erudites, set their base value to -1000.  This is barely KOS, so if you want to force more faction work to get above KOS, set is that much lower. 

See table below:  


| Faction Value | Faction CON |
| :--- | :--- |
| 1100 -&gt; ABOVE | ALLY |
| 750 -&gt; 1099 | WARMLY |
| 500 -&gt; 749 | KINDLY |
| 100 -&gt; 400 | AMIABLE |
| 0 -&gt; 99 | INDIFFERENT |
| -100 -&gt; -1 | APPREHENSIVE |
| -500 -&gt; -101 | DUBIOUS |
| -750 -&gt; -501 | THREATENLY |
| BELOW -&gt; -751 | SCOWLS |

### Create the new npc\_faction. 

Create the new entry in npc\_faction. This will be an umbrella for NPC behavior entries. Remember, this is different from the entry in faction\_list. faction\_list only identifies a core faction. npc\_faction identifies a subset of NPCs on a faction in faction\_list that have a prescribed behavior. There can be many npc\_faction entries providing different behavior for NPCs, even though all those NPCs have the same code faction\_list assignment. The key fields in npc\_faction are primary\_faction \(which you will assign to the new faction you created in step 1\) and ingnore\_primary\_assist which you will set to 1 or 0 depending on whether you want NPCs under this umbrella to assist other NPCs on the same faction\_list allegiance.

### Create new faction\_list\_mod entries to account for the Erudite loving aspect.  

So we wanted our new NPCs to like Erudites. We do this by adding an entry to faction\_list\_mod. This applies to any and all NPCs that refer back to the new faction\_list entry. So we add an entry, using the faction\_list value we created in step 1, a mod\_name \(\[rcd\]\#\) and a value. We want Erudites to be amiable to start. So we need to get them from -1000 up to at least 101. Depending on where you want them in the amiable range, the mod would be something like 1101+. So the new entry would be \(id, \(step 1 id\), 1101, r3\). Erudites are race 3.

### Create how the new npc\_faction reacts to other NPCS and PCs via npc\_faction\_entries.

 So we decided we want the NPCs under the new npc\_faction umbrella to attack other NPCs whose primary faction\_list faction is Heretic \(143\). To do this, we add an npc\_faction\_entries entry.  For us, this would be \(step 2 id, 143, 5, -1, 0\).  This indicates that all NPCs under the umbrella we created in step 2, will attack NPCs that are under any umbrella that has a primary\_faction of 143.  The -1 indicates attack.  If we changed that to 1 it would mean assist.  A 0 in that field would mean ignore.  The faction\_hit is set to +5 so that if a PC kills one of our mobs, their faction with Heretic will go up.  We also need to add a line for our own faction, so that PCs killing our NPCs will lose faction for that.  That entry would look like \(step 2 id, step 1 id, 10, 1, 0\).

As the npc\_faction\_entries documentation mentions, these table entries serve dual purpose and might be better served as separate tables.

### Assign NPCs to the new npc\_faction in the npc\_types table.

Simply change the npc\_faction\_id field for your NPCs to the new id from the second step.

### Making them fight.

Since we want these NPCs to attack other NPCs, change the npc\_types entry for any NPC assigned to this faction so npc\_aggro is set to 1.  This field must be set to enable these NPCs to agro other NPCs.

