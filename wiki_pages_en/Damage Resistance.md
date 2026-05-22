# Damage Resistance

**Damage Resistance** refers to the Bullet, Melee, and Spirit Resist statistics which reduce incoming damage taken. Bullet Resist reduces all weapon and melee damage, Melee Resist reduces only melee damage, while Spirit Resist reduces all spirit damage. Units have a unique "Damage Resistance" stat that is applied to all sources of damage, including Troopers.

Most resistances stack multiplicatively; they are not added together. Sources of Resistance Reduction are multiplied together separately first. The total reduction is then subtracted from the total resistance. This has the consequence of resistance reduction being more effective on targets with higher resistance.

## Contents

- 1 Resistance types

- 1.1 Melee Resist
- 1.2 Crit Reduction
- 2 Starting Damage Resistance
- 3 Calculation

- 3.1 Calculating Resistance
- 3.2 Calculating Resistance Reduction
- 3.3 Negative Resistance
- 4 Effective Health
- 5 Sources of Damage Resistance

- 5.1 Bullet Resist
- 5.2 Bullet Resist Reduction
- 5.3 Melee Resist
- 5.4 Spirit Resist
- 5.5 Spirit Resist Reduction

## Resistance types

[edit | edit source]

In addition to the basic types of Bullet and Spirit Resistance, there is also Melee Resist and Crit Reduction.

### Melee Resist

[edit | edit source]

Melee Resist is a stat that reduces all incoming melee damage, including from melee abilities such as  Viscous'  Puddle Punch. It increases equally to Bullet Resist (e.g. an item that gives 10% Bullet Resist also gives 10% Melee Resist). Some items also give bonus Melee Resist. Like other types of resist, it stacks multiplicatively.

### Crit Reduction

[edit | edit source]

Crit Reduction is a stat that reduces the critical damage (headshots) received by the hero. Not to be confused with Crit Bonus Scale, a stat that reduces the critical damage dealt by the hero to other targets.

## Starting Damage Resistance

[edit | edit source]

The following Heroes either have starting Damage Resistance values or gain resistance with Boons or Spirit Power. Boon and Spirit scaling resistances stack additively.

Note: Negative values indicate that the hero receives increased damage.

| Hero | Starting (%) | Added per Boon (%) | At Max Boon (%) | Spirit Scaling (%) |
| --- | --- | --- | --- | --- |
| Bebop | 0 | +0.3 | 10.5 | +0 |
| Dynamo | 0 | +0.625 | 21.9 | +0 |
| Venator | 0 | +0 | 0 | +0.122 |

| Hero | Starting (%) | Added per Boon (%) | At Max Boon (%) | Spirit Scaling (%) |
| --- | --- | --- | --- | --- |
| Kelvin | 0 | +0.625 | 21.9 | +0 |
| Lash | 10 | +0 | 10 | +0 |
| McGinnis | 0 | +0.625 | 21.9 | +0 |
| Pocket | -15 | +0 | -15 | +0 |
| Venator | 0 | +0 | 0 | +0.122 |

| Hero | Melee Resist (%) |
| --- | --- |
| Rem | -5 |

| Hero | Crit Reduction (%) |
| --- | --- |
| Mo & Krill | 20 |
| Rem | 10 |
| Seven | 35 |

## Calculation

[edit | edit source]

While items often display resistance as a flat percentage (e.g., +20% Resist), multiple sources of resistance do not simply add together. Instead, they stack **multiplicatively**.

### Calculating Resistance

[edit | edit source]

To find your total resistance, use the following formula:

Total Resist=1−(1−R1)×(1−R2)…

**Example:**
If you have two sources of resistance, one providing **40%** and another providing **20%**:

1. Convert percentages to decimals: 0.40 and 0.20.
1. Subtract from 1: (1 - 0.40) = **0.60** and (1 - 0.20) = **0.80**.
1. Multiply the remainders: 0.60 × 0.80 = **0.48**.
1. Subtract from 1: 1 - 0.48 = **0.52**.
1. Your Total Resist is **52%**.

### Calculating Resistance Reduction

[edit | edit source]

**Resistance Reduction** (often called "shred") acts as a counter to resistance. It is calculated separately using the same multiplicative formula, and then subtracted from the target's resistance.

Final Resist=Total Resistance−Total Reduction

**Example:**
A target has **52%** Total Resistance (as calculated above). You attack them with two sources of Reduction: one providing **25%** and another providing **20%**.

**Step 1: Calculate Total Reduction**
1−(1−0.25)×(1−0.20)=0.40→𝟒𝟎%

**Step 2: Subtract Reduction from Resistance**
52%−40%=𝟏𝟐%

The target has a final effective Resist of only **12%**.

### Negative Resistance

[edit | edit source]

If the Total Reduction is higher than the Total Resistance, the final value will be negative. This acts as a damage amplifier.

- **30% Resist:** You take **70%** of incoming damage.
- **0% Resist:** You take **100%** of incoming damage (True Damage).
- **-30% Resist:** You take **130%** of incoming damage.

## Effective Health

[edit | edit source]

“Alright buddy, give 'em hell!”

This page is under construction. To avoid edit conflicts, please consult the edit history and the talk page.

A graph showing how despite the resistance percentage not growing additively, it scales the player's effective health additively.

*Include graph of effective health as a function of Damage Reduction.* In the mean time, feel free to refer to this Desmos graph.

*Include graph of effective damage increase from using 15%, 30%, and 45% Resistance Reduction as a function of the target's original Damage Reduction.* In the mean time, feel free to refer to this Desmos graph.

## Sources of Damage Resistance

[edit | edit source]

### Bullet Resist

[edit | edit source]

This is an automatic list. Click here to correct the contents.

| Name | ****Cost | Category | Stat change |
| --- | --- | --- | --- |
| Fleetfoot | 1,600 | Weapon | +**6**% Bullet Resist |
| Melee Charge | 1,600 | Weapon | +**6**% Bullet Resist |
| Berserker | 3,200 | Weapon | +**8**% Bullet Resist |
| Escalating Resilience | 3,200 | Weapon | +**2**% Bullet Resist |
| Heroic Aura | 3,200 | Weapon | +**17**% Bullet Resist |
| Crushing Fists | 6,400 | Weapon | +**12**% Bullet Resist |
| Battle Vest | 1,600 | Vitality | +**18**% Bullet Resist |
| Return Fire | 1,600 | Vitality | +**10**% Bullet Resist |
| Bullet Resilience | 3,200 | Vitality | +**30**% Bullet Resist |
| Metal Skin | 3,200 | Vitality | +**12**% Bullet Resist |
| Warp Stone | 3,200 | Vitality | +**30**% Bullet Resist |
| Cheat Death | 6,400 | Vitality | +**15**% Bullet Resist |
| Indomitable | 6,400 | Vitality | +**8**% Bullet Resist |
| Siphon Bullets | 6,400 | Vitality | +**10**% Bullet Resist |
| Vampiric Burst | 6,400 | Vitality | +**10**% Bullet Resist |
| Bullet Resist Shredder | 1,600 | Spirit | +**8**% Bullet Resist |
| Suppressor | 1,600 | Spirit | +**8**% Bullet Resist |
| Superior Duration | 3,200 | Spirit | +**8**% Bullet Resist |
| Echo Shard | 6,400 | Spirit | +**5**% Bullet Resist |

- Monster Rounds increases Bullet Resist vs. NPCs by +25%.
- Escalating Resilience increases Bullet Resist by 2% per stack per shot when hitting enemy heroes, maxing at 30% Bullet Resist.

### Bullet Resist Reduction

[edit | edit source]

This is an automatic list. Click here to correct the contents.

| Name | ****Cost | Category | Stat change |
| --- | --- | --- | --- |
| Stalker | 1,600 | Weapon | -**6**% Bullet Resist Reduction |
| Weakening Headshot | 1,600 | Weapon | -**13**% Bullet Resist Reduction |
| Alchemical Fire | 3,200 | Weapon | -**7**% Bullet Resist Reduction |
| Hollow Point | 3,200 | Weapon | -**9**% Bullet Resist Reduction |
| Hunter's Aura | 3,200 | Weapon | -**10**% Bullet Resist Reduction |
| Crippling Headshot | 6,400 | Weapon | -**16**% Bullet Resist Reduction |
| Crushing Fists | 6,400 | Weapon | -**4**% Bullet Resist Reduction |
| Rusted Barrel | 800 | Spirit | -**8**% Bullet Resist Reduction |
| Bullet Resist Shredder | 1,600 | Spirit | -**10**% Bullet Resist Reduction |
| Disarming Hex | 3,200 | Spirit | -**13**% Bullet Resist Reduction |

### Melee Resist

[edit | edit source]

This is an automatic list. Click here to correct the contents.

| Name | ****Cost | Category | Stat change |
| --- | --- | --- | --- |
| Close Quarters | 800 | Weapon | +**20**% Melee Resist |
| Point Blank | 3,200 | Weapon | +**30**% Melee Resist |
| Runed Gauntlets | Legendary | Weapon | +**50**% Melee Resist |
| Rebuttal | 800 | Vitality | +**18**% Melee Resist |
| Juggernaut | 6,400 | Vitality | +**25**% Melee Resist |
| Torment Pulse | 3,200 | Spirit | +**15**% Melee Resist |

### Spirit Resist

[edit | edit source]

This is an automatic list. Click here to correct the contents.

| Name | ****Cost | Category | Stat change |
| --- | --- | --- | --- |
| Blood Tribute | 3,200 | Weapon | +**8**% Spirit Resist |
| Silencer | 6,400 | Weapon | +**15**% Spirit Resist |
| Enchanter's Emblem | 1,600 | Vitality | +**18**% Spirit Resist |
| Restorative Locket | 1,600 | Vitality | +**10**% Spirit Resist |
| Dispel Magic | 3,200 | Vitality | +**10**% Spirit Resist |
| Fury Trance | 3,200 | Vitality | +**40**% Spirit Resist |
| Spirit Resilience | 3,200 | Vitality | +**30**% Spirit Resist |
| Healing Tempo | 6,400 | Vitality | +**10**% Spirit Resist |
| Indomitable | 6,400 | Vitality | +**8**% Spirit Resist |
| Infuser | 6,400 | Vitality | +**10**% Spirit Resist |
| Spellbreaker | 6,400 | Vitality | +**18**% Spirit Resist |
| Witchmail | 6,400 | Vitality | +**20**% Spirit Resist |
| Cold Front | 1,600 | Spirit | +**6**% Spirit Resist |
| Mystic Vulnerability | 1,600 | Spirit | +**8**% Spirit Resist |
| Greater Expansion | 3,200 | Spirit | +**10**% Spirit Resist |
| Arctic Blast | 6,400 | Spirit | +**10**% Spirit Resist |
| Echo Shard | 6,400 | Spirit | +**5**% Spirit Resist |
| Escalating Exposure | 6,400 | Spirit | +**17**% Spirit Resist |
| Ethereal Shift | 6,400 | Spirit | +**30**% Spirit Resist |
| Scourge | 6,400 | Spirit | +**40**% Spirit Resist |

### Spirit Resist Reduction

[edit | edit source]

This is an automatic list. Click here to correct the contents.

| Name | ****Cost | Category | Stat change |
| --- | --- | --- | --- |
| Spirit Shredder Bullets | 1,600 | Weapon | -**8**% Spirit Resist Reduction |
| Spirit Rend | 3,200 | Weapon | -**8**% Spirit Resist Reduction |
| -**7**% Spirit Resist Reduction |  |  |  |
| Crippling Headshot | 6,400 | Weapon | -**16**% Spirit Resist Reduction |
| Spirit Strike | 800 | Spirit | -**6**% Spirit Resist Reduction |
| Mystic Vulnerability | 1,600 | Spirit | -**8**% Spirit Resist Reduction |
| Spirit Sap | 1,600 | Spirit | -**9**% Spirit Resist Reduction |
| Spirit Snatch | 3,200 | Spirit | -**12**% Spirit Resist Reduction |
| Escalating Exposure | 6,400 | Spirit | -**8**% Spirit Resist Reduction |
| Focus Lens | 6,400 | Spirit | -**9**% Spirit Resist Reduction |

- Spirit Rend reduces -8% spirit resist on bullet hit from its component  Spirit Shredder Bullets, as well as an additional -7% spirit resist reduction per stack on headshots, up to a max of 4 stacks (-33% spirit resist total).

| | Stats |  | | --- | --- | | Weapon | Ammo •  Bullet Damage •  Bullet Velocity •  Damage per second •  Falloff Range •  Fire Rate •  Melee Damage •  Melee Distance •  Reload Time •  Weapon Damage | | Vitality | Bullet Evasion •  Damage Barrier •  Damage Resistance •  Debuff Resist •  Health •  Health Regen •  Healing •  Lifesteal •  Movement Slow •  Move Speed •  Slide Distance •  Stamina | | Spirit | Ability Cooldown •  Ability Duration •  Ability Range •  Bonus Ability Charges •  Imbue •  Spirit Damage •  Spirit Power •  Spirit Scaling | | Other | Abilities •  Build-Up •  Charge-Up •  Damage Amplification •  Hero Attributes Table •  Pure Damage •  Scaling •  Stack | |
| --- |