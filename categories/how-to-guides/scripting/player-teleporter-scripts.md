# Player Teleporter Scripts

Below is an example of a quest script for an NPC that can teleport your players. Ths scripts would go in your quest scripts directory, and would be named appropriately based on the NPC that you will create to transport your players.

## Old World Porter

This script will name translocate targets and teleport your player based on the target of their choosing.

{% code title="Roald\_Teavee.pl" %}
```perl
sub EVENT_SAY {
	if ($text =~ /Hail/i) {
		quest::say("Hello. $name!  I am practicing the arcane art of [" . quest::saylink("teleportation") . "].  Would you like to try teleporting?");
	}
	elsif ($text =~ /teleportation/i) {
		quest::say("I have mastered teleporting adventurers to [" . quest::saylink("Antonica") . "], [" . quest::saylink("Faydwer") . "], and [" . quest::saylink("Odus") . "].  Where would you like to travel?");
	}
	elsif ($text =~ /Antonica/i) {
		quest::say("I have mastered transport to [" . quest::saylink("Nektulos Forest") . "], [" . quest::saylink("The Northern Desert of Ro") . "], [" . quest::saylink("The Northern Plains of Karana") . "], [" . quest::saylink("The Temple of Cazic Thule") . "], [" . quest::saylink("The Western Commonlands") . "]and [" . quest::saylink("The Western Plains of Karana") . "].  Where would you like to go?");
	}
	elsif ($text =~ /Faydwer/i) {
		quest::say("I have mastered transport to [" . quest::saylink("The Greater Faydark") . "].  Where would you like to go?");
	}
	elsif ($text =~ /Odus/i) {
		quest::say("I have mastered transport to [" . quest::saylink("Toxxulia Forest") . "].  Where would you like to go?");
	}
	elsif ($text =~ /Nektulos Forest/i) {
		quest::say("Begone!");
		$npc->CastSpell(1371, $userid);
	}
	elsif ($text =~ /The Northern Desert of Ro/i) {
		quest::say("Begone!");
		$npc->CastSpell(1373, $userid);
	}
	elsif ($text =~ /The Northern Plains of Karana/i) {
		quest::say("Begone!");
		$npc->CastSpell(1338, $userid);
	}
	elsif ($text =~ /The Temple of Cazic Thule/i) {
		quest::say("Begone!");
		$npc->CastSpell(1375, $userid);
	}
	elsif ($text =~ /The Western Commonlands/i) {
		quest::say("Begone!");
		$npc->CastSpell(1372, $userid);
	}
	elsif ($text =~ /The Western Plains of Karana/i) {
		quest::say("Begone!");
		$npc->CastSpell(1374, $userid);
	}
	elsif ($text =~ /The Greater Faydark/i) {
		quest::say("Begone!");
		$npc->CastSpell(1336, $userid);
	}
	elsif ($text =~ /Toxxulia Forest/i) {
		quest::say("Begone!");
		$npc->CastSpell(1337, $userid);
	}

}

sub EVENT_ITEM {
	#:: Return unused items
	plugin::returnUnusedItems();
}
```
{% endcode %}

