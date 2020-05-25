# Expansions and Content Quest API

This highlights contextual Quest API calls that are relevant to expansions design

### Use Case Examples

1\) We have an NPC that existed already in for example expansion 4; **Planes of Power** but a few expansion down the line, the dialogue of this NPC has changed. We need a boolean or conditional that we can check to see what current expansion context the server is in before making behavioral changes in our script

```perl
if (quest::is_current_expansion_dragons_of_norrath()) {
    # New Quest Dialogue
    if ($text=~/hail/i) {
        # Some text
    }
}
```

2\) We a good handful of classic zones; later down the line in **Lost Dungeons of Norrath** we get these messages when entering the zones

> A mysterious voice whispers to you, 'If you can feel me in your thoughts, know this -- something is changing in the world and I reckon you should be a part of it. I do not know much, but I do know that in every home city and the wilds there are agents of an organization called the Wayfarers Brotherhood. They are looking for recruits . . . If you can hear this message, you are one of the chosen. Rush to your home city, or search the West Karanas and Rathe Mountains for a contact if you have been exiled from your home for your deeds, and find out more. Adventure awaits you, my friend.''

Before these new additions there was nothing to conditionally check which expansion was enabled or disabled to determine whether or not to even display this message, which could be solved with the addition of **the following call.** If we set our server to an earlier expansion these messages would disappear 

```perl
eq.is_lost_dungeons_of_norrath_enabled()
```

What this looks like in the **global\_player.lua**

{% code title="global\_player.lua" %}
```lua
function event_enter_zone(e)
	local qglobals = eq.get_qglobals(e.self);
	if(e.self:GetLevel() >= 15 and qglobals['Wayfarer'] == nil and eq.is_lost_dungeons_of_norrath_enabled()) then
		local zoneid = eq.get_zone_id();
		if(e.self:GetStartZone() ~= zoneid and (zoneid == 1 or zoneid == 2 or zoneid == 3 or zoneid == 8 or zoneid == 9 
		or zoneid == 10 or zoneid == 19 or zoneid == 22 or zoneid == 23 or zoneid == 24 or zoneid == 29 or zoneid == 30 
		or zoneid == 34 or zoneid == 35 or zoneid == 40 or zoneid == 41 or zoneid == 42 or zoneid == 45 or zoneid == 49 
		or zoneid == 52 or zoneid == 54 or zoneid == 55 or zoneid == 60 or zoneid == 61 or zoneid == 62 or zoneid == 67 
		or zoneid == 68 or zoneid == 75 or zoneid == 82 or zoneid == 106 or zoneid == 155 or zoneid == 202 or zoneid == 382 
		or zoneid == 383 or zoneid == 392 or zoneid == 393 or zoneid == 408)) then
			e.self:Message(15, 
				"A mysterious voice whispers to you, \'If you can feel me in your thoughts, know this -- "
				.. "something is changing in the world and I reckon you should be a part of it. I do not know much, but I do know "
				.. "that in every home city and the wilds there are agents of an organization called the Wayfarers Brotherhood. They "
				.. "are looking for recruits . . . If you can hear this message, you are one of the chosen. Rush to your home city, or "
				.. "search the West Karanas and Rathe Mountains for a contact if you have been exiled from your home for your deeds, "
				.. "and find out more. Adventure awaits you, my friend.\'");
		end
	end
end
```
{% endcode %}

## Expansions Quest API

{% tabs %}
{% tab title="Lua" %}
```lua
eq.is_classic_enabled()
eq.is_the_ruins_of_kunark_enabled()
eq.is_the_scars_of_velious_enabled()
eq.is_the_shadows_of_luclin_enabled()
eq.is_the_planes_of_power_enabled()
eq.is_the_legacy_of_ykesha_enabled()
eq.is_lost_dungeons_of_norrath_enabled()
eq.is_gates_of_discord_enabled()
eq.is_omens_of_war_enabled()
eq.is_dragons_of_norrath_enabled()
eq.is_depths_of_darkhollow_enabled()
eq.is_prophecy_of_ro_enabled()
eq.is_the_serpents_spine_enabled()
eq.is_the_buried_sea_enabled()
eq.is_secrets_of_faydwer_enabled()
eq.is_seeds_of_destruction_enabled()
eq.is_underfoot_enabled()
eq.is_house_of_thule_enabled()
eq.is_veil_of_alaris_enabled()
eq.is_rain_of_fear_enabled()
eq.is_call_of_the_forsaken_enabled()
eq.is_the_darkend_sea_enabled()
eq.is_the_broken_mirror_enabled()
eq.is_empires_of_kunark_enabled()
eq.is_ring_of_scale_enabled()
eq.is_the_burning_lands_enabled()
eq.is_torment_of_velious_enabled()
eq.is_current_expansion_classic()
eq.is_current_expansion_the_ruins_of_kunark()
eq.is_current_expansion_the_scars_of_velious()
eq.is_current_expansion_the_shadows_of_luclin()
eq.is_current_expansion_the_planes_of_power()
eq.is_current_expansion_the_legacy_of_ykesha()
eq.is_current_expansion_lost_dungeons_of_norrath()
eq.is_current_expansion_gates_of_discord()
eq.is_current_expansion_omens_of_war()
eq.is_current_expansion_dragons_of_norrath()
eq.is_current_expansion_depths_of_darkhollow()
eq.is_current_expansion_prophecy_of_ro()
eq.is_current_expansion_the_serpents_spine()
eq.is_current_expansion_the_buried_sea()
eq.is_current_expansion_secrets_of_faydwer()
eq.is_current_expansion_seeds_of_destruction()
eq.is_current_expansion_underfoot()
eq.is_current_expansion_house_of_thule()
eq.is_current_expansion_veil_of_alaris()
eq.is_current_expansion_rain_of_fear()
eq.is_current_expansion_call_of_the_forsaken()
eq.is_current_expansion_the_darkend_sea()
eq.is_current_expansion_the_broken_mirror()
eq.is_current_expansion_empires_of_kunark()
eq.is_current_expansion_ring_of_scale()
eq.is_current_expansion_the_burning_lands()
eq.is_current_expansion_torment_of_velious()
```
{% endtab %}

{% tab title="Perl" %}
```
quest::is_classic_enabled()
quest::is_the_ruins_of_kunark_enabled()
quest::is_the_scars_of_velious_enabled()
quest::is_the_shadows_of_luclin_enabled()
quest::is_the_planes_of_power_enabled()
quest::is_the_legacy_of_ykesha_enabled()
quest::is_lost_dungeons_of_norrath_enabled()
quest::is_gates_of_discord_enabled()
quest::is_omens_of_war_enabled()
quest::is_dragons_of_norrath_enabled()
quest::is_depths_of_darkhollow_enabled()
quest::is_prophecy_of_ro_enabled()
quest::is_the_serpents_spine_enabled()
quest::is_the_buried_sea_enabled()
quest::is_secrets_of_faydwer_enabled()
quest::is_seeds_of_destruction_enabled()
quest::is_underfoot_enabled()
quest::is_house_of_thule_enabled()
quest::is_veil_of_alaris_enabled()
quest::is_rain_of_fear_enabled()
quest::is_call_of_the_forsaken_enabled()
quest::is_the_darkend_sea_enabled()
quest::is_the_broken_mirror_enabled()
quest::is_empires_of_kunark_enabled()
quest::is_ring_of_scale_enabled()
quest::is_the_burning_lands_enabled()
quest::is_torment_of_velious_enabled()
quest::is_current_expansion_classic()
quest::is_current_expansion_the_ruins_of_kunark()
quest::is_current_expansion_the_scars_of_velious()
quest::is_current_expansion_the_shadows_of_luclin()
quest::is_current_expansion_the_planes_of_power()
quest::is_current_expansion_the_legacy_of_ykesha()
quest::is_current_expansion_lost_dungeons_of_norrath()
quest::is_current_expansion_gates_of_discord()
quest::is_current_expansion_omens_of_war()
quest::is_current_expansion_dragons_of_norrath()
quest::is_current_expansion_depths_of_darkhollow()
quest::is_current_expansion_prophecy_of_ro()
quest::is_current_expansion_the_serpents_spine()
quest::is_current_expansion_the_buried_sea()
quest::is_current_expansion_secrets_of_faydwer()
quest::is_current_expansion_seeds_of_destruction()
quest::is_current_expansion_underfoot()
quest::is_current_expansion_house_of_thule()
quest::is_current_expansion_veil_of_alaris()
quest::is_current_expansion_rain_of_fear()
quest::is_current_expansion_call_of_the_forsaken()
quest::is_current_expansion_the_darkend_sea()
quest::is_current_expansion_the_broken_mirror()
quest::is_current_expansion_empires_of_kunark()
quest::is_current_expansion_ring_of_scale()
quest::is_current_expansion_the_burning_lands()
quest::is_current_expansion_torment_of_velious()
```
{% endtab %}
{% endtabs %}

## Content Flag Quest API

{% tabs %}
{% tab title="Lua" %}
```lua
eq.is_content_flag_enabled(string flag_name);
eq.set_content_flag(string flag_name, bool enabled);
```
{% endtab %}

{% tab title="Perl" %}
```
quest::is_content_flag_enabled(string flag_name);
quest::set_content_flag(string flag_name, bool enabled);
```
{% endtab %}
{% endtabs %}

