# Fire Rate

Fire Rate, also known as **Bullets per second**, is a stat that determines the amount of ammo that will be fired by the weapon per second. Several heroes have abilities that can increase their fire rates to shoot faster, but it can also be decreased, primarily through other enemy's items.

The inverse of this is called *gun cycle time*, which instead measures **seconds per bullet**.

## Contents

- 1 Math

- 1.1 Examples

- 1.1.1 Combined Bonuses and Slows
- 1.1.2 Maximum Slow Reduction
- 2 Base Fire Rate
- 3 Sources

- 3.1 Fire Rate
- 3.2 Fire Rate Slow
- 3.3 Map spawns

## Math

[edit | edit source]

The final Fire Rate change is calculated with separate rules for bonuses and slows: positive bonuses (buffs) are additive, while negative modifiers (slows) are multiplicative.

It is important to note that the total change to Fire Rate cannot be reduced below **-50%**. Any calculated value lower than this will be capped at -50%.

The simplified formula is:

Fire Rate Modifier=(Sum of Bonuses)−(1−Total Slows)

Where:

- **Sum of Bonuses** = All positive buffs added together (e.g., 0.25+0.20)
- **Total Slows** = The result of multiplying the remaining values of each slow: (1−Slow1)×(1−Slow2)×…

### Examples

[edit | edit source]

#### Combined Bonuses and Slows

[edit | edit source]

For an example with multiple sources:

- **+25%** Fire Rate from  Ricochet
- **+20%** Fire Rate from  Swift Striker
- **-25%** Fire Rate Slow from  Sinclair's  Vexing Bolt
- **-35%** Fire Rate Slow from an enemy's  Suppressor

First, calculate the groups separately:

- **Bonuses:** 0.25+0.20=0.45
- **Slows:** (1−0.25)×(1−0.35)=0.75×0.65=0.4875

Then combine them in the final formula:

Final=0.45−(1−0.4875)
Final=0.45−0.5125=−0.0625

This results in a **-6.25%** final change. The in-game UI typically rounds this value to the nearest whole number, displaying **-6%**.

#### Maximum Slow Reduction

[edit | edit source]

For an example with only slows applied:

- No positive Fire Rate bonuses (0)
- **-25%** Fire Rate Slow from  Sinclair's  Vexing Bolt
- **-35%** Fire Rate Slow from an enemy's  Suppressor

The calculation is:

0−(1−(0.75×0.65))
0−(1−0.4875)=−0.5125

This results in a calculated slow of **-51.25%**. Due to the cap, this value is raised to the maximum reduction of **-50%**.

## Base Fire Rate

[edit | edit source]

Values referenced from Hero Comparison Table.

Note:  McGinnis' and  Victor's weapons have a wind-up time before reaching maximum fire rate.

| Hero | Rounds/s | Spirit Scaling |
| --- | --- | --- |
| Abrams | 1.59 | +0 |
| Apollo | 2.63 | +0 |
| Bebop | 11.9 | +0 |
| Billy | 11.8 | +0 |
| Calico | 4.76 | +0 |
| Celeste | 1.72 | +0 |
| The Doorman | 1.59 | +0 |
| Drifter | 2.27 | +0 |
| Dynamo | 3.81 | +0 |
| Graves | 9.8 | +0 |
| Grey Talon | 1.73 | +0 |
| Haze | 9.52 | +0 |
| Holliday | 2.12 | +0 |
| Infernus | 9.52 | +0 |
| Ivy | 13.6 | +0 |
| Kelvin | 3.81 | +0 |
| Lady Geist | 2.12 | +0 |
| Lash | 5.83 | +0 |
| McGinnis | 4.76 | +0 |
| Mina | 3.97 | +0 |
| Mirage | 2.72 | +0 |
| Mo & Krill | 5.29 | +0 |
| Paige | 2 | +0 |
| Paradox | 7.56 | +0 |
| Pocket | 1.9 | +0 |
| Rem | 3.85 | +0 |
| Seven | 5.83 | +0 |
| Shiv | 1.81 | +0 |
| Silver | 1.11 | +0 |
| Silver (Transformed) | 2 | +0 |
| Sinclair | 2.72 | +0 |
| Venator | 7.94 | +0 |
| Victor | 5.05 | +0 |
| Vindicta | 4.33 | +0 |
| Viscous | 4.76 | +0 |
| Vyper | 14.3 | +0 |
| Warden | 3.81 | +0.01 |
| Wraith | 10.6 | +0 |
| Yamato | 2.38 | +0 |

| Hero | Rounds/s |
| --- | --- |
| Shiv | 0.794 |
| Viscous | 0.794 |
| Yamato | 0.952 |

## Sources

[edit | edit source]

### Fire Rate

[edit | edit source]

This is an automatic list. Click here to correct the contents.

| Name | ****Cost | Category | Stat change |
| --- | --- | --- | --- |
| Rapid Rounds | 800 | Weapon | +**9**% Fire Rate |
| Active Reload | 1,600 | Weapon | +**25**% Fire Rate |
| Kinetic Dash | 1,600 | Weapon | +**25**% Fire Rate |
| Swift Striker | 1,600 | Weapon | +**20**% Fire Rate |
| Blood Tribute | 3,200 | Weapon | +**35**% Fire Rate |
| Burst Fire | 3,200 | Weapon | +**10**% Fire Rate |
| +**32**% Fire Rate |  |  |  |
| Heroic Aura | 3,200 | Weapon | +**26**% Fire Rate |
| Shadow Weave | 3,200 | Weapon | +**20**% Fire Rate |
| Capacitor | 6,400 | Weapon | +**5**% Fire Rate |
| Frenzy | 6,400 | Weapon | +**15**% Fire Rate |
| +**40**% Fire Rate |  |  |  |
| Ricochet | 6,400 | Weapon | +**18**% Fire Rate |
| Spellslinger | 6,400 | Weapon | +**11**% Fire Rate |
| Spiritual Overflow | 6,400 | Weapon | +**32**% Fire Rate |
| Infinite Rounds | Legendary | Weapon | +**35**% Fire Rate |
| Battle Vest | 1,600 | Vitality | +**7**% Fire Rate |
| Fury Trance | 3,200 | Vitality | +**30**% Fire Rate |
| Healing Tempo | 6,400 | Vitality | +**35**% Fire Rate |
| Vampiric Burst | 6,400 | Vitality | +**34**% Fire Rate |
| Quicksilver Reload | 1,600 | Spirit | +**10**% Fire Rate |
| Surge of Power | 3,200 | Spirit | +**20**% Fire Rate |
| Echo Shard | 6,400 | Spirit | +**5**% Fire Rate |
| Focus Lens | 6,400 | Spirit | +**10**% Fire Rate |
| Mercurial Magnum | 6,400 | Spirit | +**22**% Fire Rate |
| Shrink Ray | Legendary | Spirit | +**20**% Fire Rate |

- Burst Fire additionally increases Fire Rate by +32%% for 4.5 seconds after hitting an enemy hero.
- Heroic Aura's Fire Rate bonus is doubled for nearby player minions within its 30m radius.

### Fire Rate Slow

[edit | edit source]

This is an automatic list. Click here to correct the contents.

| Name | ****Cost | Category | Stat change |
| --- | --- | --- | --- |
| Hunter's Aura | 3,200 | Weapon | +**14**% Fire Rate Slow |
| Juggernaut | 6,400 | Vitality | +**36**% Fire Rate Slow |
| Rusted Barrel | 800 | Spirit | +**32**% Fire Rate Slow |
| Suppressor | 1,600 | Spirit | +**28**% Fire Rate Slow |

### Map spawns

[edit | edit source]

- Golden Statues can provide a permanent increase: +**1.5**% Fire Rate before 10 minutes, +**2**% Fire Rate before 30 minutes, or +**2.5**% Fire Rate after 30 minutes.
- Powerup runes can provide a temporary Gun buff that provides +**12**% to +**35**% Fire Rate for 160 seconds (scaling with game time from 5 to 40 minutes).

| | Stats |  | | --- | --- | | Weapon | Ammo •  Bullet Damage •  Bullet Velocity •  Damage per second •  Falloff Range •  Fire Rate •  Melee Damage •  Melee Distance •  Reload Time •  Weapon Damage | | Vitality | Bullet Evasion •  Damage Barrier •  Damage Resistance •  Debuff Resist •  Health •  Health Regen •  Healing •  Lifesteal •  Movement Slow •  Move Speed •  Slide Distance •  Stamina | | Spirit | Ability Cooldown •  Ability Duration •  Ability Range •  Bonus Ability Charges •  Imbue •  Spirit Damage •  Spirit Power •  Spirit Scaling | | Other | Abilities •  Build-Up •  Charge-Up •  Damage Amplification •  Hero Attributes Table •  Pure Damage •  Scaling •  Stack | |
| --- |