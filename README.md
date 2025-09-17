
# Tank Compendium - Project Epoch

<br>

# Warrior

<br>

## Talents

With the uncertainty of how incoming raids will be tuned, these talent builds rely on using a shield (i know, right?).


<br>

[**Standard build**](https://mel-talent-calc.vercel.app/warrior/350003011-05-0055511033010103501351/0BAFH1B2CEDGIJNFlPQSTUV)
* Cookie cutter def build.

<br>

[**Demo Shout build**](https://mel-talent-calc.vercel.app/warrior/340003-055-0055511033010101501351/0AF1BC2CDEGFIlJNpQSTUV)
* Build with imp demo shout to reduce the damage taken. This is especially useful unless you can rely on other warriors to provide imp demo shout or hunters with owls/bats (screech).

<br>

[**Impale build**](https://mel-talent-calc.vercel.app/warrior/35000301302-03-0055511033010101501351/0AFHIBK2CDEGIlFNJpQSTUV1bbb)
* Recommended for geared tanks with at least 18% critical strike chances before buffs, which is the threshold where trading 2 points from  Cruelty to activate  Impale instead becomes a small threat increase. 
* Impale also significantly increases your damage output when not tanking, which is a nice bonus for an off-tank.


<br>

## Stats

**Notable talent/stat synergies**

* Vitality: +10% Strength, +5% Stamina ⇒ more AP, more block value & HP. 
* Toughness: +10% armor from items (multiplicative with other armor buffs). 
* Anticipation: +20 Defense skill (huge toward crit immunity at 60). 
* Shield Mastery: +30% block value → more mitigation and Shield Slam damage/threat. 
* Defiance: +15% threat and +6 expertise. 
---

### Primary Stats

#### Stamina

* Stamina → Health. Above the first 20 Stamina, 1 Stam ≈ 10 HP. Warrior talents Vitality give +5% total Stamina (5/5), so your Stamina is multiplied before converting to HP.
* Both Tauren Racial (Endurance) and Mining Passive (Toughness?) - +5% total Stamina each - multiplies your whole post-Stamina HP, and also scales any flat HP.
* HP formula :
<br> 
    * > HP = (Base HP + 10 x (Stam x 1.05vitality)) x 1.05 endurance x 1.05 mining  
    (...include Kings/fort/etc. where relevant)

#### Strength

* Strength → 2 AP per 1 Str and block value at +1 block value per 20 Strength (in Classic/TBC). Block value reduces damage on blocks and also boosts Shield Slam damage. Shield Mastery multiplies your total block value by +30%.

#### Agility

* Agility → armor, crit, dodge. Simple rules of thumb at lvl 60: 1 Agi = 2 armor; roughly ~30 Agi ≈ 1% dodge and ~33 Agi ≈ 1% crit for Prot Warrior (ratings era numbers; exact class/level scaling varies).

#### Intellect/Spirit

* Minimal value for Prot (mana/regen only).

<br>
<br>

### Secondary stats & ratings

#### Armor
* Physical DR -> DR = Armor / (Armor + K).
* For bosses (level 63), solving for 75% DR gives an armor cap around 17,265 in Classic/TBC-era formulas. <br> (Use K ≈ 400 + 85 × AttackerLevel at 1–59; special 60+ constants exist—community math lands you near that 17.2k number vs 63.) 

#### Defense skill
* You need 440 Defense skill to be crit-immune vs L63 (5.6% crit to remove; each Defense skill above attacker reduces crit chance by 0.04%).
* Anticipation (Prot) gives +20 Defense skill by itself. 

### Block rating/value.
* Block chance comes from block rating/defense. 
* Block value reduces hit size and fuels Shield Slam. 
* Shield Block and Shield Mastery scale your block value (and Slam) multiplicatively. 

#### Expertise
* Each 1 expertise reduces enemy dodge and parry by 0.25%. 
* Prot gets +6 expertise skill from Defiance (3/3) in TBC. 

#### Hit Chance

**Bosses are level 63**: melee special hit cap is ~8% (9% “on gear”).


<br>
<br>

## Threat 

### Core rules (what threat is)

* Every mob keeps a threat table. Whoever has the most threat is the target (unless taunted, stunned, etc.). Melee DPS must exceed the tank by 110% to pull; ranged must exceed by 130%. 
* Damage → threat at 1 threat per 1 damage (before multipliers).
* Healing generates 0.5 threat per point of effective healing, and that healing threat is evenly split among all enemies you’re in combat with. Overheal is 0 threat.
* “Power gains” like rage from Bloodrage / potions generate threat (≈ 5 threat per 1 rage) and stance/form threat multipliers do not affect this.
* Threat modifiers (stance/form, talents, Salvation, etc.) are multiplicative with each other.

<br>

> **Disclaimer**: There is a lot of custom rework on classes for Project Epoch, and some numbers may vary. <br>
>In the time of writing, there is also a lot of issues with all classes and abilities, and some of these spells/abilities might not work as intended for the time being..

<br>
<br>

<br>

### Built-in multipliers as a Protection Warrior

* **Defensive Stance**: ×1.30 to almost all threat you cause.

* **Defiance (3/3)**: +15% more on top → 1.30 × 1.15 = 1.495× to your ability/damage threat (multiplier). (Battle/ Berserker Stance are ×0.8.) 
>Multipliers are multiplicative with everything else (Salv, etc.).

<br>

### Ability-by-ability

* **Shield Slam** Threat = (damage) (scales with Block Value) + an innate flat bonus, then × modifier.

* **Devastate** threat ≈ (50% normalized weapon damage + 35×stacks damage) + +101 innate threat, then × modifier; with 5 stacks that worked out to ~444 raw before stance.
>**Patch 2.3**: Devastate “combines the effects of Sunder Armor” and is affected by all talents/items that affect Sunder—i.e., when you add a Sunder via Devastate you also get Sunder’s flat threat; refreshing at 5 stacks does not add a new Sunder.

* **Sunder Armor**: Flat +301 threat per application (Rank 6) with no damage; multiply by modifier. Still generates threat even past 5 stacks (but doesn’t stack further).

* **Revenge**: Cheap, off-CD when it lights: damage + a flat bonus (rank-based; commonly ~+200 at level-70 ranks) → then × modifier. Pound it whenever it procs.

* **Heroic Strike**: Adds damage and a flat +196 threat (Rank 10) to that swing, then × modifier. Remember: HS replaces the rage you’d gain from that white hit, so it’s only efficient when you’ve got spare rage.

* **Thunder Clap**: Base threat = 1.75 × damage done, then × modifier. In TBC it hits up to 4 targets. Use it for opener “glue,” not for sustained AoE TPS.

* **Demoralizing Shout**: Very small fixed threat (treat it as utility/mitigation, not real TPS).

* **Taunt**: Sets your threat equal to the current target’s highest (no bonus), then forces attacks for 3s. Follow it with a big threat move (Shield Slam/Devastate).

<br>

### Quick Math

Modifier = 1.495 (Defensive + Defiance).
* **Generic hit** (no special bonus): Threat = Damage × 1.495. 

* **Sunder**: Threat = 301 × 1.495 = 450 per GCD. 

* **Devastate** (5 stacks, 2.0.x baseline): ~444 × 1.495 ≈ 664 per GCD. If you apply a Sunder with Devastate (2.3+), add Sunder’s flat threat before multiplying. 

* **Shield Slam** (example): if it hits for 800 and we use ~+300 flat: (800 + 300) × 1.495 ≈ 1,645 threat. 

* **Revenge** (example): if it hits for 400 and we assume ~+200 flat: (400 + 200) × 1.495 ≈ 898 threat.

* **Heroic Strike** (example swing): if HS adds +176 damage and +196 threat and your swing’s post-mitig damage add is 400 → (400 + 196) × 1.495 ≈ 894 threat (but account for HS rage cost/opportunity).

* **Thunder Clap** (example): if it deals 120 to each of 4 mobs: per mob 120 × 1.75 × 1.495 ≈ 314 threat (cap 4 targets). 

<br>

### Threat examples with math

#### Single-target boss opener (no external buffs)

Assume: Shield Slam hits for 800; Devastate at 5 stacks; Revenge lights; Sunder as needed.

* **Shield Slam**: (800 + ~300) × 1.495 ≈ 1,645 threat. 

* **Devastate (5 stacks)**: ~444 × 1.495 ≈ 664 threat (refresh only). If this GCD adds a Sunder stack (2.3+), add +301 × 1.495 ≈ 450 more. 

* **Revenge**: (~400 + ~200) × 1.495 ≈ 898 threat. 

* **Fillers**: Sunder (≈450) when Devastate isn’t optimal (e.g., building early stacks) or you’re rage-starved; HS only if you’re floating rage. 

> Practical prio: Shield Slam on CD → Revenge on proc → Devastate (build/maintain stacks) → Sunder only while stacking / if you can’t Devastate → HS to bleed excess rage.


#### 5-mob trash pull (glue + tab threat)

* **Thunder Clap** hits 4 targets for ~120 → ~314 threat each (×1.495, 1.75x base), then tab Devastate/Sunder the kill target and runner; Demo Shout for mitigation + a bit of blanket threat; Taunt anything that peels and follow with Shield Slam. 

---

<br>
<br>
<br>
<br>

# Paladin

<br>

## Talents

With the uncertainty of how incoming raids will be tuned, these talent builds rely on using a shield (i know, right?).


<br>

[**Deep Prot build**](https://mel-talent-calc.vercel.app/paladin/-0530513300050152521051-050050013/1BECFGLNooooQPSRUV2BEI1H2H1o)
* Avenger’s Shield build.

<br>

[**Imp Sanctity Aura**](https://mel-talent-calc.vercel.app/paladin/-053050300005013252103-052050113003012/1BECGLNQPSRuuu2BEIHgCLNO)
* Sanctity Aura build.

<br>

[**Vengeance build**](https://mel-talent-calc.vercel.app/paladin/-0530503000050130501-0500505130030125/1BECGLNQS2BEIHLNOGP)
* Sanctity Aura build with Vengeance.


<br>

## Stats

**Notable talent/stat synergies**

* Divine Strength (+15% Str) → more AP and block value.
* Sacred Duty (+6% Stamina) + Combat Expertise (+10% Stamina) → very efficient EH scaling.
* Anticipation (+20 Defense skill) → pushes you toward crit immunity.
* One-Handed Weapon Spec (+5% dmg) and Improved Righteous Fury → much stronger threat & 6% DR (with 3/3).
---

### Primary Stats

#### Stamina

* Stamina → Health. **Sacred Duty** (2/2) = +6% total Stamina; **Combat Expertise** (5/5) = +10% total Stamina. These are Stamina multipliers (they happen before Stam → HP).
* Both Tauren Racial (Endurance) and Mining Passive (Toughness?) - +5% total Stamina each - multiplies your whole post-Stamina HP, and also scales any flat HP.
* HP formula :
<br> 
    * > HP = (Base HP + 10 x (Stam x 1.06SD x 1.10CE)) x 1.05 endurance x 1.05 mining  
    (...include Kings/fort/etc. where relevant)

#### Strength

* Strength → 2 AP per 1 Str and block value +1 per 20 Str. Divine Strength (5/5) gives +15% Strength.

#### Agility

* Agility → armor/crit/dodge (same general notes as Warrior; Agi is nice for avoidance and crit for Seal/Judge procs, but your TPS core is Holy damage).

#### Intellect/Spirit

* Intellect → mana & spell crit. Larger blue bar + more spell crit for Holy Shield/Avenger’s Shield/Seal/Judgement scaling; Divine Intellect adds +10% Intellect.

<br>
<br>

### Secondary stats & ratings

#### Spell Damage
* Spell damage directly scales Consecration, Holy Shield damage, Avenger’s Shield, Seal/Judgement of Righteousness, etc. (your AoE threat backbone at 60). 
* One-Handed Weapon Spec (+5% damage) and Improved Righteous Fury (+90% threat, and up to 6% damage reduction at 3/3) are key.

#### Armor
* Physical DR -> DR = Armor / (Armor + K).
* For bosses (level 63), solving for 75% DR gives an armor cap around 17,265 in Classic/TBC-era formulas. <br> (Use K ≈ 400 + 85 × AttackerLevel at 1–59; special 60+ constants exist—community math lands you near that 17.2k number vs 63.) 

#### Defense skill
* You need 440 Defense skill to be crit-immune vs L63 (5.6% crit to remove; each Defense skill above attacker reduces crit chance by 0.04%).
* Anticipation (Prot) gives +20 Defense skill by itself. 

### Block rating/value.
* Redoubt (proc block chance), Holy Shield gives huge block chance (and deals damage on blocks). 
* Strength increases block value (mitigation) but Holy Shield’s damage scales primarily with spell coefficients. 

#### Expertise
* Each 1 expertise reduces enemy dodge and parry by 0.25%. 
* Combat Expertise also grants +5 expertise (i.e., −1.25% dodge/parry combined), improving white/special connects for SoR/JoR melee pieces and Avengers swings.

#### Hit chance

**Bosses are level 63**: melee special hit cap is ~8% (9% “on gear”), while spells (e.g., Avenger’s Shield) use the **spell hit table** (effective cap ~16% vs L63), so AS will “miss/resist” more often unless you gear some spell hit.




<br>
<br>

## Threat


### Core rules (what threat is)

* Every mob keeps a threat table. Whoever has the most threat is the target (unless taunted, stunned, etc.). Melee DPS must exceed the tank by 110% to pull; ranged must exceed by 130%. 
* Damage → threat at 1 threat per 1 damage (before multipliers).
* Healing generates 0.5 threat per point of effective healing, and that healing threat is evenly split among all enemies you’re in combat with. Overheal is 0 threat.
* “Power gains” like rage from Bloodrage / potions generate threat (≈ 5 threat per 1 rage) and stance/form threat multipliers do not affect this.
* Threat modifiers (stance/form, talents, Salvation, etc.) are multiplicative with each other.

<br>

> **Disclaimer**: There is a lot of custom rework on classes for Project Epoch, and some numbers may vary. <br>
>In the time of writing, there is also a lot of issues with all classes and abilities, and some of these spells/abilities might not work as intended for the time being..


<br>
<br>

### Built-in multipliers as a Protection Paladin
* **Righteous Fury (RF)**: +60% threat to Holy spells (×1.6). With Improved Righteous Fury 3/3 it increases RF’s bonus by 50%, i.e., +90% total → ×1.9 to (most) Holy-based threat. (It also gives 6% damage taken reduction.)

* **Holy Shield** damage has +35% extra threat baked in (on top of RF). (Base Holy Shield has 4 charges; Improved Holy Shield adds +2/+4 charges and +10/20% damage.)

> Multiplying it all: for a Holy spell without its own bonus, Threat = Damage × 1.9 (with Imp RF). For Holy Shield, Threat = Damage × 1.35 × 1.9.

### Ability-by-ability

* **Consecration** — 8-sec ground DoT, 8 ticks (1/sec). Threat is pure damage (Holy) → ×1.9 with RF. (Rank 1 is cheap and still benefits from RF.)

* **Holy Shield** — Each block deals Holy damage and gets +35% threat and RF. Your highest TPS when getting hit fast.

* **Avenger’s Shield** — Snap ranged Holy damage on up to 3 targets; great opener. Threat = damage × RF. (Rank 3 deals 494–602 per target before mods.)

* **Seal + Judgement**

  * **Seal of Righteousness (SoR)** — Adds Holy damage to every swing; Judgement of Righteousness is direct Holy damage. Threat = damage × RF.

  * **Seal of Vengeance (SoV)** — (Alliance in original TBC; widely available in TBC Classic) stacks a Holy DoT; strong single-target threat when stacked. DoT + Judgement = Holy → RF applies.

* **Retribution Aura** — Deals small Holy damage to attackers; every hit is Holy → ×1.9. (TBC guides often quote 26 damage/hit at max rank → ~49 threat/hit with RF.)

* **(Greater) Blessing of Sanctuary** — When you block, the attacker takes small Holy damage (and you reduce damage taken); Holy damage → ×1.9.

* **Righteous Defense** — Multi-target taunt (no damage, no direct threat added) that sets your threat to the current highest for those mobs and forces attacks for 3s.

* **Misc Holy nukes (situational)**: Exorcism/Holy Wrath (undead/demon only) → damage × RF.

> Patch talent that quietly helps: One-Handed Weapon Specialization (Prot) became “increases all damage by up to 5%”, which bumps your damage (and thus threat) across the board.

<br>

### Pre-healing & self-heals: how they affect threat

* Heals done before combat starts = 0 threat, because you aren’t on any mob’s table yet.

* Heals that land after you’re on the table generate 0.5 threat per effective heal, split evenly across all mobs you’re in combat with.

* With RF up, Paladin Holy spells (including heals) contribute increased threat—so if you Flash of Light yourself after you’ve engaged, you’ll generate extra healing threat while RF is active. (Rule of thumb many use: treat it as “healing threat × 1.9” in TBC with Imp RF.) 

<br>
<br>

### Threat examples with math

>Assumptions for the math below (swap in your actual hits):
> * RF with Imp RF 3/3 → ×1.9 to Holy.
> * Holy Shield has +35% threat on its damage.
> * Sample values are illustrative only.

<br>

#### Single-target opener (boss)

* **Avenger’s Shield** hits for 550 → Threat = 550 × 1.9 = **1,045**. 
* **Consecration** (8s) ticks for 150 each × 8 = 1,200 damage → Threat = 1,200 × 1.9 = **2,280**. 
* **Holy Shield**: 3 blocks in the first 10s at 155 each → raw dmg 465. Threat = 465 × 1.35 × 1.9 = **1,191**.
* **Judgement of Righteousness** hits for 300 → Threat = 300 × 1.9 = **570**.

> Rough total over the first 8–10s: ~5,086 threat → ~510 TPS (heavily dependent on blocks and your actual numbers).

#### 5-mob AoE pull

* **Consecration** ticks 150 each → 285 threat per tick per mob (×1.9). Over 8s, **2,280 threat per mob**.

* **Avenger’s Shield** tags 3 mobs for **550 each** → **1,045* opening threat to those 3.

* **Holy Shield**: say you consume 8 charges in 10s at 155 each → damage 1,240 → Threat = 1,240 × 1.35 × 1.9 ≈ **3,176**, distributed to whatever is swinging (great front-loaded TPS).

* **Retribution Aura**: if each mob hits you once per sec for 8s at 26 aura damage per hit → 26 × 1.9 ≈ **49 threat/hit**. With 5 mobs × 8s ≈ ~1,960 extra splash threat riding passively. (Real hit timers vary.)

* **Blessing of Sanctuary**: each block returns small Holy damage → multiply its damage by 1.9 for the threat per block.

> Practical opener: AS → Consecration → Holy Shield (keep it up) → Judge on the runner → maintain seal. Toss Righteous Defense if anything peels (it sets your threat to the leader on that target).

---

<br>
<br>
<br>
<br>

# Druid

<br>

## Talents



<br>

[**Standard PvE DPS/Tank Hybrid Build**](https://mel-talent-calc.vercel.app/druid/-503032132322105301251-05503301/2BCEH1AECFGHKJIMLOPRSTU2F)
* This is the standard PvE build that the vast majority of feral druids should take regardless of whether they primarily tank or primarily DPS in their raid team.

<br>

[**Demo Roar Tank/DPS Hybrid Build**](https://mel-talent-calc.vercel.app/druid/-553032132322105301051-05503001/2BCEH1AECFGHKJIMLOPRTUB)
* This build gives up **Improved Leader of the Pack** and  **Intensity** in order to pick up 5/5 **Feral Aggression**. Use this in the event that your raid team lacks warriors Demoralizing Shout.

<br>

[**PvP Tank Talent Build**](https://mel-talent-calc.vercel.app/druid/01-503202132322125331051-05503001/2BCEH1ACFGHKJIMLOPRTUD0B1NQ)
* This build picks up **Brutal Impact**, **Nurturing Instinct**, and **Primal Tenacity**. It also takes a single point in the Balance tree for **Nature's Grasp**.


<br>


## Stats

**Notable talent/stat synergies**

* Heart of the Wild and Dire Bear together super-charge Stamina; SotF adds +3% stats and −3% crit taken.
* Thick Hide (3/3) adds +10% armor from items, stacking with Dire Bear’s multiplier.
* Weapon AP is replaced by Feral Attack Power on druid weapons.
* Strength/Agility and armor are your main levers.
---

### Primary Stats

#### Stamina

* Stamina → Health. Bears get very large Stamina multipliers:
    * Dire Bear Form: +25% Stamina baseline (and a massive armor multiplier from leather).
    * Heart of the Wild (5/5): +20% Stamina in Bear/Dire Bear.
    * Survival of the Fittest (3/3): +3% to all attributes (so Stamina +3%), and −3% chance to be critically hit. (This talent does not by itself make you crit-immune at level 60; you still need additional Defense/Resilience to meet the ~5.6% boss crit reduction.)
* Both Tauren Racial (Endurance) and Mining Passive (Toughness?) - +5% total Stamina each - multiplies your whole post-Stamina HP, and also scales any flat HP.
* HP formula :
<br> 
    * > HP = (Base HP + 10 x (Stam x 1.03SotF x 1.20HotW x 1.25DireBear)) x 1.05 endurance x 1.05 mining  
    (...include Kings/Mark/fort/etc. where relevant)

#### Strength

* Strength → 2 AP per 1 Str in Bear. (Agility does not add AP to Bear; that’s Cat-only.)

#### Agility

* Agility → armor, crit, dodge. 1 Agi = 2 armor, plus strong dodge/crit for Bears. Agility is excellent for mitigation and threat (crit → Maul/Lacerate TPS), but Stamina/EH is king at 60.


<br>
<br>

### Secondary stats & ratings

#### Armor
* Armor multipliers: Dire Bear Form multiplies armor from leather by roughly ~4× (patch texts vary by era; many references list ~+400% from items). Thick Hide (3/3) adds +10% armor from items on top. These stack multiplicatively and make Bears the kings of physical DR at 60. 

#### Defense skill
* Bosses have ~5.6% chance to crit (+3 levels). SotF gives −3%, so you still need −2.6% from Defense skill. At level 60 with ratings: 1.5 Defense rating = 1 Defense skill, and 25 Defense skill ≈ −1% crit.

#### Block rating/value.
* Can’t block or parry. You live on Armor + Dodge + Big Health.

#### Expertise
* Each 1 expertise reduces enemy dodge and parry by 0.25%.

#### Hit chance

* Bosses are level 63: melee special hit cap is ~8% (9% “on gear”).

### Stat Weights

| Stat                   | Normalized Weight |
| ---------------------- | ----------------: |
| Attack Power           |                 1 |
| Feral Attack Power     |                 1 |
| Strength               |             2.266 |
| Agility                |               4.6 |
| Hit Rating             |               3.5 |
| Expertise Rating       |               7.3 |
| Critical Strike Rating |               1.9 |
| Haste Rating           |               1.6 |
| Armor Penetration      |              0.34 |
| Stamina                |              3.05 |
| Armor                  |              0.59 |
| Defense Rating         |               2.2 |
| Dodge Rating           |               1.7 |



<br>
<br>

## Threat

### Core rules (what threat is)

* Every mob keeps a threat table. Whoever has the most threat is the target (unless taunted, stunned, etc.). Melee DPS must exceed the tank by 110% to pull; ranged must exceed by 130%. 
* Damage → threat at 1 threat per 1 damage (before multipliers).
* Healing generates 0.5 threat per point of effective healing, and that healing threat is evenly split among all enemies you’re in combat with. Overheal is 0 threat.
* “Power gains” like rage from Bloodrage / potions generate threat (≈ 5 threat per 1 rage) and stance/form threat multipliers do not affect this.
* Threat modifiers (stance/form, talents, Salvation, etc.) are multiplicative with each other.

<br>

> **Disclaimer**: There is a lot of custom rework on classes for Project Epoch, and some numbers may vary. <br>
>In the time of writing, there is also a lot of issues with all classes and abilities, and some of these spells/abilities might not work as intended for the time being..

<br>
<br>


### Built-in multipliers as a feral tank

* **Bear/Dire Bear Form**: ×1.30 threat to all your damage-based threat.

* **Feral Instinct (3/3)**: ×1.15 more threat (applies only in bear forms).
Together, bears sit at 1.30 × 1.15 = 1.495× threat on all damage-based sources.

> **Note**: these multipliers do not change healing/mana/rage-gain threat—those are unmodified. 

<br>

### Ability-by-ability

Below is what each ability does for threat in TBC. “Damage × Modifier” means “whatever damage the ability deals, multiply the resulting threat by 1.495 - assuming you have the Feral Instinct talent.”

* **Mangle (Bear)**: No extra threat modifier. Threat = damage × modifier. It also debuffs the target so all bleeds (and Shred) deal +30% damage for 12s, which passively boosts Lacerate-tick threat. 

* **Lacerate**: On application it has a flat bonus threat (TBC value widely documented as +285 before multipliers) plus its small direct damage; both are then multiplied by modifier. The DoT ticks (15s total, 5 ticks every 3s) are ordinary bleed damage → threat (and are 30% stronger while Mangle’s debuff is up). 

* **Maul**: A “next-swing” strike with a flat bonus threat per rank added to its damage, then × modifier. (TBC changed Maul from Classic’s weird multiplier to a rank-based flat threat bonus.) Threat math is (Maul damage + Maul bonus) × modifier. 

* **Swipe (Bear)**: No innate bonus threat in TBC; it’s just damage → threat (× modifier). Also, it hits up to 3 targets in TBC (not 360°/uncapped until Wrath). 

* **Faerie Fire (Feral)**: Costs 0 rage, does (AP×0.15 + 1) damage, and has additional built-in threat in bear forms. Treat it as (damage + internal bonus) × modifier; it’s one of your best GCDs for snap threat on cooldown. 

* **Demoralizing Roar**: Tiny threat; use it for mitigation, not TPS. (Any threat it gives is negligible compared to Mangle/Lacerate/Maul/Swipe.)

* **Thorns**: Every reflected tick is just damage → threat, multiplied by your bear modifiers like any damage you deal. (Great passive AoE glue early in a pull.) 

* **Growl (taunt)**: Sets your threat equal to the current target’s highest threat; it doesn’t add threat by itself and isn’t multiplied. Use it to match the leader, then follow with a high-threat ability. 

### How pre-HoTs (self-healing before the pull) affect threat

* If you cast Rejuvenation/Regrowth/Lifebloom on yourself before pulling, the ticks that occur after combat begins generate 0.5 threat per point of effective healing, split evenly across all mobs you’re in combat with, and not multiplied by bear/stance/talents.

* That means on a big pack, pre-HoTs give you a small, instant spread of threat on everything—useful “glue” while your first Swipes/Mangles go out. (Overheal ticks are 0 threat.) 

> **Example (pre-HoT)**: Rejuvenation tick heals you for 800 effective right after you body-pull a 4-mob pack → total healing threat = 800×0.5 = 400, split 400/4 = 100 threat on each mob (unmodified by bear multipliers).

<br>

### Threat examples with math



#### Single-target opener (no external buffs)

#### Assume:
* Your Mangle hits for 1,200.
* You apply Lacerate (100 direct damage, +285 bonus threat).
* You queue Maul and it hits for 900; assume Maul’s flat bonus ≈ +200 (rank-based in TBC).

#### Threat per GCD:
* Mangle: 1,200 × 1.495 = **1,794 threat**. 
* Lacerate (application): (100 + 285) × 1.495 = **576 threat**. 
* Maul: (900 + 200) × 1.495 ≈ **1,645 threat**. 


Immediate total after those three actions ≈ **4,015 TPS** worth of lead (not counting white swings).

Lacerate over time: Suppose your Lacerate DoT totals 600 damage baseline over 15s; with Mangle’s +30% bleed debuff it does 780 total = 156 per tick (5 ticks). Each tick’s threat: 156 × 1.495 ≈ **233**; over 15s that’s ~**1,166 extra threat** “for free.” 

<br>

#### 5-mob trash pull (using pre-HoTs + Swipe)

* Pre-pull Rejuvenation tick lands for 700 effective right as combat starts → healing threat = 700×0.5 = 350 total, split 350/5 = **70 per mob** (unmodified). 

* Swipe hits 3 targets; assume 300 damage to each → per target threat = 300 × 1.495 = 449. Two Swipes (tagging different 3-packs) quickly give you **~900 threat** on five mobs, while the pre-HoT glued them at 70 each and Thorns ticks add small, multiplied damage-threat as they swing. (Remember Swipe hits 3 targets in TBC.)

<br>
<br>

### Practical threat priorities (TBC)

#### Single target

* Keep Mangle on cooldown (biggest snap TPS).
* Stack/maintain Lacerate to 5, then refresh; its +285 on apply plus buffed bleed ticks are huge over time.
* Maul when you have the rage (it’s off-GCD and carries a flat threat bonus).
* Faerie Fire (Feral) on cooldown for free, high snap threat and armor debuff.

#### Multi-target (3+)

* Swipe on cooldown and tab-Mangle through priority targets; sprinkle Lacerate on ones you risk losing. Remember Swipe is 3-target in TBC, so rotate it smartly.

* Pre-HoT yourself and keep Thorns up for passive spread threat on entry.

* Use Growl to match a runner’s top threat, then Mangle/Maul to leap ahead.

<br>
<br>

### Reference: threat formulas

* **Generic hit**: Threat = (Damage) × 1.495 (bear + Feral Instinct). 

* **Lacerate (apply)**: ((DirectDamage) + 285) × 1.495. DoT ticks: (TickDamage) × 1.495. 

* **Maul**: ((MaulDamage) + MaulFlatBonusByRank) × 1.495. (Flat bonus is rank-based in TBC.) 

* **Mangle**: (Damage) × 1.495. Also remember Mangle → +30% bleed damage (bakes more Lacerate tick-threat). 

* **Faerie Fire (Feral)**: ((AP×0.15 + 1) + internal bonus) × 1.495.

* **Healing tick after pull**: (EffectiveHeal × 0.5) / (#mobs in combat with you). Not multiplied by bear/talents.

* **Rage gains (e.g., pot, Enrage tick)**: Rage × 5 threat (unmodified by form/talents).
---
<br>
<br>

