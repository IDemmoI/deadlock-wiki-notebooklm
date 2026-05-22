# Healing

**Healing** is the act of recovering a unit's current health, which includes various methods such as Lifesteal, Health Regen, and Item effects.

## Contents

- 1 Healing Amp
- 2 Healing Reduction
- 3 Calculation

- 3.1 Calculating Healing Reduction
- 3.2 Calculating Final Healing
- 4 Sources of direct healing

- 4.1 Heroes
- 4.2 Items
- 5 Sources of healing reduction

- 5.1 Heroes
- 5.2 Items
- 6 See also

## Healing Amp

[edit | edit source]

Healing Amp, also known as Healing Effectiveness, is a stat which increases the amount of healing a hero does with their abilities and items. This affects both healing to themselves and to their allies. Healing Amp affects healing-over-time buffs, such as  Healing Rite's active effect.

This stat is represented as a percentage. For example, a 25% gain would increase a heal of 100 to 125.

## Healing Reduction

[edit | edit source]

Healing Reduction is a negative effect which reduces the effectiveness of healing on the unit it is applied to.

Healing Reduction is represented as a percentage and stacks multiplicatively, meaning each additional source has diminishing returns.

If a player is hit by the same source of Healing Reduction before its effect has worn off (e.g. two or more enemy players with  Healbane), only the first source is applied.

## Calculation

[edit | edit source]

### Calculating Healing Reduction

[edit | edit source]

Multiple sources of Healing Reduction stack **multiplicatively**:

Total Reduction=1−(1−R1)×(1−R2)…

**Example:**
If two sources of Healing Reduction are applied, one providing **40%** and another providing **40%**:

1. Convert percentages to decimals: 0.40 and 0.40.
1. Subtract from 1: (1 - 0.40) = **0.60** and (1 - 0.40) = **0.60**.
1. Multiply the remainders: 0.60 × 0.60 = **0.36**.
1. Subtract from 1: 1 - 0.36 = **0.64**.
1. Total Healing Reduction is **64%**, not 80%.

### Calculating Final Healing

[edit | edit source]

Final Healing=Initial Healing×(1−Total Reduction)×(1+Healing Amp)

**Example:**
A heal of **200 HP** is applied to a target with **64%** Total Healing Reduction. The healer has **25%** Healing Amp.

1. Apply Reduction: 200 × (1 - 0.64) = 200 × 0.36 = **72 HP**.
1. Apply Amp: 72 × (1 + 0.25) = 72 × 1.25 = **90 HP**.
1. Final Healing received is **90 HP**.

Note: Healing from self-damage sources such as  Victor's  Pain Battery and  Aura of Suffering does not appear in the endgame hero stats screen, but it does appear in the healing sources graph.

## Sources of direct healing

[edit | edit source]

Killing a Medic Trooper drops a Medic Pack that heals nearby players based on the following formula:

*Heal = (12% of hero's missing HP + 150 HP + 2 HP per minute) / Number of nearby heroes*

### Heroes

[edit | edit source]

This is an automatic list. Click here to add notes or correct the contents.

| Hero | Ability | Notes |
| --- | --- | --- |
| Abrams | Siphon Life | Lifesteals off damage dealt while active. |
| Abrams | Infernal Resilience | Passively restores health for a percentage of all incoming damage. |
| Apollo | Flawless Advance | Heals a flat amount per hit. Unlocked by T1 upgrade. |
| Bebop | Exploding Uppercut | Restores a portion of missing health on use. Unlocked by T3 upgrade. |
| Calico | Leaping Slash | Heals a flat amount on hero hit. Unlocked by T1 upgrade. |
| Calico | Return to Shadows | Heals a flat amount on use. Unlocked by T3 upgrade. |
| Celeste | Light Eater | Grants a buff that gives spirit lifesteal while active. |
| Drifter | Bloodscent | Restores a portion of missing health on kill. |
| Dynamo | Rejuvenating Aurora | Heals per second while channeling. T3 upgrade also adds passive max health regen. |
| Grey Talon | Rain of Arrows | Grants bullet and spirit lifesteal while active. Unlocked by T3 upgrade. |
| Infernus | Napalm | Lifesteals off all damage dealt to napalmed targets. Unlocked by T2 upgrade. |
| Infernus | Concussive Combustion | Lifesteals off damage dealt. Unlocked by T2 upgrade. |
| Ivy | Kudzu Connection | Grants bullet lifesteal. Also replicates a portion of healing. |
| Ivy | Stone Form | Heals a percentage of max HP on cast. |
| Kelvin | Frost Grenade | Heals Kelvin and nearby allies for a flat amount. |
| Kelvin | Frozen Shelter | Regenerates health for all allies inside the dome. |
| Lash | Flog | Heals Lash for a percentage of damage dealt to heroes. |
| McGinnis | Medicinal Specter | Heals nearby allies per second. |
| Mina | Rake | Heals a flat amount on kill. |
| Mo & Krill | Scorn | Heals for a percentage of damage dealt. |
| Mo & Krill | Combo | Lifesteals off damage dealt. Unlocked by T1 upgrade. |
| Paige | Rallying Charge | Heal affected allies and Paige for a flat amount. |
| Rem | Tag Along | Restores a portion of target's missing health on attachment, then heals per second for a short duration. |
| Rem | Lil Helpers | Regenerates health for any trooper the helpers are attached to. |
| Silver | Lycan Curse | Restores a percentage of missing health on activation. |
| Silver (Transformed) | Go For The Throat | Lifesteals off melee damage dealt. |
| Victor | Pain Battery | Restores a portion of missing health on hero hit. Unlocked by T3 upgrade. |
| Victor | Jumpstart | Grants a flat health regen buff on use. |
| Viscous | The Cube | Regenerates health for the target. |
| Warden | Last Stand | Lifesteals off all damage dealt while active. |
| Wraith | Card Trick | Heals Wraith for a flat amount when a Heart or Joker card hits. |
| Yamato | Crimson Slash | Heals a flat amount on hero hit. |
| Yamato | Shadow Transformation | Restores a percentage of max health per hero kill. |

### Items

[edit | edit source]

| Name | **** Cost | Category | Healing amount |
| --- | --- | --- | --- |
| Restorative Shot | 800 | Weapon | 50 Healing From Heroes 15 Healing From NPCs |
| Headhunter | 3,200 | Weapon | 4% *x*0.06 Heal Per Headshot |
| Healing Rite | 800 | Vitality | 300 *x*0.93 Total HP Regen |
| Melee Lifesteal | 800 | Vitality | 100 Heal on Melee Hit (30% on NPCs) |
| Healbane | 1,600 | Vitality | 275 Heal On Hero Kill |
| Restorative Locket | 1,600 | Vitality | 16 *x*0.32 Heal Per Stack |
| Healing Nova | 3,200 | Vitality | 325 *x*6 Total HP Regen |
| Lifestrike | 3,200 | Vitality | 100 *x*1.5 Heal on Melee Hit, plus 30% *x*0.5 Lifesteal (40% on NPCs) |
| Rescue Beam | 3,200 | Vitality | 20% Heal Amount |
| Siphon Bullets | 6,400 | Vitality | Max HP Steal Per Bullet |
| Radiant Regeneration | 3,200 | Spirit | 70 *x*2 Heal on Ability Cast |

## Sources of healing reduction

[edit | edit source]

### Heroes

[edit | edit source]

This is an automatic list. Click here to add notes or correct the contents.

| Hero | Ability | Heal Reduction | Notes |
| --- | --- | --- | --- |
| Drifter | Stalker's Mark | 40% (T3) | — |
| Infernus | Napalm | 33% (T3) | — |
| Pocket | Affliction | 100% (T3) | — |
| Venator | Consecrating Grenade | 30% | T3 upgrade increases heal reduction by 20% (total 50%). |
| Vindicta | Crow Familiar | 35% (T1) | — |
| Vyper | Lethal Venom | 40% (T2) | — |

### Items

[edit | edit source]

This is an automatic list. Click here to correct the contents.

| Name | ****Cost | Category | Stat change |
| --- | --- | --- | --- |
| Toxic Bullets | 3,200 | Weapon | -**35**% Healing Reduction |
| Crippling Headshot | 6,400 | Weapon | -**35**% Healing Reduction |
| Haunting Shot | Legendary | Weapon | -**40**% Healing Reduction |
| Healbane | 1,600 | Vitality | -**35**% Healing Reduction |
| Cheat Death | 6,400 | Vitality | -**60**% Healing Reduction |
| Inhibitor | 6,400 | Vitality | -**40**% Healing Reduction |
| Decay | 3,200 | Spirit | -**50**% Healing Reduction |
| Spirit Burn | 6,400 | Spirit | -**70**% Healing Reduction |

- Cheat Death applies **-60%** healing reduction to its user for 4.5 seconds (the same duration as the invulnerability).

## See also

[edit | edit source]

- Bullet Lifesteal
- Spirit Lifesteal
- Health Regen

| | Stats |  | | --- | --- | | Weapon | Ammo •  Bullet Damage •  Bullet Velocity •  Damage per second •  Falloff Range •  Fire Rate •  Melee Damage •  Melee Distance •  Reload Time •  Weapon Damage | | Vitality | Bullet Evasion •  Damage Barrier •  Damage Resistance •  Debuff Resist •  Health •  Health Regen •  Healing •  Lifesteal •  Movement Slow •  Move Speed •  Slide Distance •  Stamina | | Spirit | Ability Cooldown •  Ability Duration •  Ability Range •  Bonus Ability Charges •  Imbue •  Spirit Damage •  Spirit Power •  Spirit Scaling | | Other | Abilities •  Build-Up •  Charge-Up •  Damage Amplification •  Hero Attributes Table •  Pure Damage •  Scaling •  Stack | |
| --- |

| | Gameplay |  | | --- | --- | | General | Abilities • Glossary • Heroes • Hideout • Items • Map • Skill Rating • Stats • Strategy • Street Brawl | | Map features | Cosmic Veil • Crate • The Curiosity Shop • Golden Statue • Jump pad • Mid-Boss • Neutrals • Powerup • Rejuvenator • Ropes • Sinner's Sacrifice • Soul Urn • Structures • Teleporter • Vent • Ziplines | | Mechanics | Backdoor Protection • Boon • Cheater Frog • Crowd Control • Death • Extra Slots • Health • Melee Attack • Minimap • Movement • Souls • Stack • Status Effects | |
| --- |