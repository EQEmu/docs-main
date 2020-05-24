# Spell Damage Modifiers

**Overview of spell effects that modify Spell Damage**

**Key: Focus Effect,** _**Item Effect**_**,** ~~**Non-Focus Spell Effect**~~

_\*Spell damage criticals are not a flat \(2x\) they are determined soely by your 'critical damage modifer' value._

_\*If multiple of same Focus Effect, highest avialable value is used. \[Stacks\] Indicates that if multiple of same effect, the final amount is the total of all effects._ 

**Direct Damage**

* **Focus Effects** **that increase/decrease damage by percent.**
  * **SE\_FcBaseEffects \(413\)** Modifies by % the base damage value of the spell cast.
  * **SE\_ImprovedDamage** **\(124\)** Modifies by % the damage value after \(413\) is applied. \(This value CAN NOT critical\)
  * **SE\_FcDamagePctCrit \(302\)** Modifies by % the damage value after \(413\) is applied. \(This value CAN critical\)
* **Effects on CASTER that increase/decrease damage by a specific amount.**
  * **SE\_FcDamageAmt \(286\)** +/- a set damage amount \(This value CAN NOT criticals\).
  * **SE\_FcDamageAmtCrit \(303\)** +/- a set damageamount \(This value CAN critical\)
  * _**Item 'Spell Damage Amount"**_ - Amount specified on the item modified by formula bellow \(This value CAN critical\)
    * Value is modified by the 'total cast time' of the spell it is being applied to
    * _Total Cast Time_ is derived from adding which ever is greater\(Recast OR Recovery time\) to cast time.
    * _Total Cast Time_ \(0 - 2.5 seconds\). 
      * Damage Amount = Damagel Amount / 4
    * _Total Cast Time_ \(2.6 - 7.0 seconds\)
      * Damage Amount = Damage Amount\*\(0.167\*\(_Total Cast Time_\)/1000\)\)
    * _Total Cast Time_ \( &gt; 7.0 seconds\)
      * Damage Amount = Damage Amount / 7
* **Effects on TARGET that increase/decrease damage by a specific amount.**
  * **SE\_FcDamageAmtIncoming \(297\)** +/- a set amount of damage \(This value CAN NOT critical\)
* **Effects on TARGET that increase/decrease damage  by percent.**
  * **SE\_FcSpellVulnerability \(296\)**  Modifies by % the casters base damage value \(This value CAN critical\).
* **Effects on CASTER that increase/decrease critical spell chance.** 
  * ~~**SE\_CriticalSpellChance \(294\)**~~ ****Modfies by % the chance to critical spell chance AND critical damage modifer. \[c_ritcal portion_ Stacks\]
  * ~~**SE\_SpellCritChance \(170\)**~~ Modifies by % the chance to critical spell. \[Stacks\]
  * ~~**SE\_FrenziedDevastation \(212\)**~~ ****Modifies by % the chance to critical spells AND increases DD spells mana cost by 2x \[Stacks\]
* **Effects on CASTER that increase/decrease critical spell damage. \(**_**Critcal Spell Damage Modifier**_**\)**
  * ~~**SE\_CriticalSpellChance \(294\)**~~ ****Modfies by % the chance to critical spell chance AND critical damage modifer. \[_damage portion does not Stack_\]
  * ~~**SE\_SpellCritDmgIncrease \(155\)**~~ ****Modifies by % the critical damage modifier. \[Stacks\]

**Calculation** 

**Critical Chance =** ~~**SE\_CriticalSpellChance**~~ **+** ~~**SE\_SpellCritChance**~~ **+** ~~**SE\_FrenziedDevastation**~~

**X =** Damage Amount

**CritMod** =  ~~**SE\_CriticalSpellChance**~~ **+** ~~**SE\_SpellCritDmgIncrease**~~

**Final Damage Amount = \( \(X \* SE\_FcBaseEffects\) \* SE\_ImprovedDamage \) +**  **\(\(X \* SE\_FcBaseEffects\) \* FcDamagePctCrit \)\*CritMod\) +  SE\_FcDamageAmt + \(SE\_FcDamageAmtCrital \* CritMod\) + \(**_**Item 'Spell Damage Amount"**_ **\* CritMod\) + SE\_FcDamageAmtIncoming +  \(\(\(X \* SE\_FcBaseEffects\) \* SE\_FcSpellVulnerability \)\* CritMod\)\)\)** 

**DAMAGE OVER TIME**

_\*Critcal damage modifer for DOTs is always \(2x\) at baseline if you have a chance to critical._

* **Focus Effects** **that increase/decrease damage by percent.**
  * **SE\_FcBaseEffects \(413\)** Modifies by % the base damage value of the spell cast.
  * **SE\_ImprovedDamage** **\(124\)** Modifies by % the damage value after \(413\) is applied. \(This value CAN critical\) _\*Unlike DD spells this does critical for DOTS_
  * **SE\_FcDamagePctCrit \(302\)** Modifies by % the damage value after \(413\) is applied. \(This value CAN critical\)
* **Effects on CASTER that increase/decrease damage by a specific amount.**  _\*Damage is divided by duration and that value is applied to each tick_
  * **SE\_FcDamageAmt \(286\)** +/- a set damage amount \(This value CAN NOT criticals\).
  * **SE\_FcDamageAmtCrit \(303\)** +/- a set damageamount \(This value CAN critical\)
  * _**Item 'Spell Damage Amount"**_ \* Not applied to DOTS
* **Effects on TARGET that increase/decrease damage by a specific amount.** _\*Damage is divided by duration and that value is applied to each tick_
  * **SE\_FcDamageAmtIncoming \(297\)** +/- a set amount of damage \(This value CAN NOT critical\)
* **Effects on TARGET that increase/decrease damage by percent.**
  * **SE\_FcSpellVulnerability \(296\)**  Modifies by % the casters base damage value \(This value CAN critical\).
* **Effects on CASTER that increase/decrease critical dot chance.** 
  * ~~**SE\_CriticalDotChance \(273\)**~~ ****Modfies by % the chance to critical dot hance  \[Stacks\]
  * ~~**SE\_CriticalDotlDecay \(433\)**~~ ****Modifies by % the chance to critical dots. \[Stacks\]
    *  Effect value decreases if spell cast is over the maximum level specified.
* **Effects on CASTER that increase/decrease critical dot damage. \(**_**Critical Spell Damage Modifier**_**\)**
* **SE\_DotCritDmgIncrease \(375\)** Modifies by % the critical damage modifier. \[Stacks\]

**Calculation** 

**Critical Chance =** ~~**SE\_CriticalDotChance**~~ **+** ~~**SE\_CriticalDotDecay**~~ ****

**X =** Damage Amount

**CritMod** = ~~**Baseline\(100%\)**~~ **+** ~~**SE\_DotCritDmgIncrease**~~

**Final DOT Damage Amount = \( \(X \* SE\_FcBaseEffects\) \* SE\_ImprovedDamage \) +  \(\(X \* SE\_FcBaseEffects\) \* FcDamagePctCrit \)\*CritMod\) +  \(\(SE\_FcDamageAmt + \(SE\_FcDamageAmtCrital \* CritMod\)**

**+ SE\_FcDamageAmtIncoming\)/DURATION\) +  \(\(\(X \* SE\_FcBaseEffects\) \* SE\_FcSpellVulnerability \)\* CritMod\)\)\)** 

