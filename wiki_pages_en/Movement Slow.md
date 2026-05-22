# Movement Slow

**Movement Slow** is a status effect applied by many items and abilities that slows move speed by a percentage.

Movement Slow cannot reduce a player's speed below 2.0 m/s in-game (or 80 hammer units per second).

## Contents

- 1 Notes
- 2 Calculation

- 2.1 Stacking Multiple Slows
- 2.2 Calculating Final Speed
- 2.3 Movement Slow Resist
- 3 Sources

- 3.1 Heroes
- 3.2 Items
- 3.3 Movement Slow Resist

- 3.3.1 Heroes
- 3.3.2 Items

## Notes

[edit | edit source]

- The displayed speed in-game in m/s is rounded to the nearest decimal for all numbers under 10 m/s.

## Calculation

[edit | edit source]

### Stacking Multiple Slows

[edit | edit source]

While abilities and items display slow percentages (e.g., 30%), multiple sources of movement slow do not simply add together. Instead, they stack **multiplicatively**.

To find your total slow percentage, use the following formula:

Total Slow=1−(1−Slow1)×(1−Slow2)×...

**Example:**
If you are affected by two slows, one providing **30%** and another providing **25%**:

1. Convert percentages to decimals: 0.30 and 0.25.
1. Subtract from 1: (1 - 0.30) = **0.70** and (1 - 0.25) = **0.75**.
1. Multiply the remainders: 0.70 × 0.75 = **0.525**.
1. Subtract from 1: 1 - 0.525 = **0.475**.
1. Your Total Slow is **47.5%**.

### Calculating Final Speed

[edit | edit source]

Once you have the total slow percentage, apply it to your speed. However, movement slow is calculated using 2.0 m/s as a floor - you cannot be slowed below this speed.

Slowed Speed=((Current Speed−2)×(1−Total Slow))+2

**Example:**
If you are moving at **10 m/s** and have **50%** total slow:

1. Subtract the floor: 10 - 2 = **8**.
1. Apply the slow: 8 × (1 - 0.50) = 8 × 0.50 = **4**.
1. Add the floor back: 4 + 2 = **6 m/s**.

### Movement Slow Resist

[edit | edit source]

Movement Slow Resist reduces the final calculated slow percentage. Multiple sources of Movement Slow Resist stack **additively** (not multiplicatively).

Actual Slow=Total Slow×(1−Resist1−Resist2−...)

**Example:**
If you have **47.5%** total slow and **30%** Movement Slow Resist:
47.5%×(1−0.30)=47.5%×0.70=𝟑𝟑.𝟐𝟓%

## Sources

[edit | edit source]

“If we are to complete the ritual, we must think clearly.”

This page may contain **factual inaccuracies**. The information presented requires verification against reliable sources.

Issue: *List may be outdated, numbers need to be automated*

#### Heroes

[edit | edit source]

This is an automatic list. Click here to add notes or correct the contents.

| Hero | Ability | Move Slow | Notes |
| --- | --- | --- | --- |
| Abrams | Shoulder Charge | 40% (T1) | — |
| Apollo | Disengaging Sigil | 30% | — |
| Bebop | Grapple Arm | 90% | Applies a short strong slow when the victim reaches Bebop. |
| Bebop | Hyper Beam | 25% | — |
| Celeste | Shining Wonder | 40% | T1 upgrade increases move slow by 20% (total 60%). |
| Dynamo | Kinetic Pulse | 30% (T2) | — |
| Graves | Jar of Dead | 30% (T2) | — |
| Graves | Borrowed Decree | 80% | — |
| Grey Talon | Rain of Arrows | 40% (T2) | — |
| Grey Talon | Spirit Snare | 30% | — |
| Haze | Sleep Dagger | 50% (T3) | — |
| Haze | Fixation | 15% (T1) | — |
| Infernus | Napalm | 35% | — |
| Ivy | Entangling Thorns | 35% | — |
| Ivy | Air Drop | 40% (T2) | — |
| Kelvin | Frost Grenade | 40% | — |
| Kelvin | Arctic Beam | 20% | T1 upgrade increases move slow by 25% (total 45%). Also slows the caster for 8%. |
| Kelvin | Frozen Shelter | 35% | — |
| Lady Geist | Malice | 15% | — |
| Lady Geist | Soul Exchange | 70% | — |
| Lash | Ground Strike | 50% (T2) | — |
| Lash | Flog | 35% (T1) | — |
| Lash | Death Slam | 50% | — |
| McGinnis | Spectral Wall | 20% | T3 upgrade increases move slow by 30% (total 50%). |
| McGinnis | Heavy Barrage | 30% (T1) | Slows McGinnis by unknown amount. |
| Mina | Love Bites | 30% (T1) | — |
| Mirage | Dust Devil | 30% | — |
| Mirage | Djinn's Mark | 60% (T1) | — |
| Mo & Krill | Sand Blast | 25% (T2) | — |
| Paige | Captivating Read | 45% | — |
| Paradox | Pulse Grenade | 20% | — |
| Paradox | Time Wall | 80% | — |
| Pocket | Barrage | 30% | — |
| Pocket | Enchanter's Satchel | 40% (T3) | — |
| Seven | Lightning Ball | 35% (T2) | — |
| Shiv | Serrated Knives | 35% | — |
| Silver | Entangling Bola | 20% | T1 upgrade increases move slow by 25% (total 45%). |
| Silver (Transformed) | Tail Whack | 30% | T2 upgrade increases move slow by 40% (total 70%). |
| The Doorman | Call Bell | 35% | — |
| Victor | Pain Battery | 40% (T1) | — |
| Victor | Aura of Suffering | 25% (T1) | — |
| Victor | Shocking Reanimation | 120% | — |
| Vindicta | Stake | 40% | — |
| Viscous | Splatter | 35% | — |
| Viscous | Puddle Punch | 20% | — |
| Vyper | Screwjab Dagger | 35% | — |
| Vyper | Petrifying Bola | 50% | — |
| Warden | Alchemical Flask | 20% | — |
| Wraith | Card Trick | 30% | T3 upgrade increases move slow by 20% (total 50%). |
| Wraith | Telekinesis | 40% | — |
| Yamato | Power Slash | 40% (T1) | — |
| Yamato | Flying Slash | 50% | — |

#### Items

[edit | edit source]

This is an automatic list. Click here to correct the contents.

| Name | ****Cost | Category | Stat change |
| --- | --- | --- | --- |
| Slowing Bullets | 1,600 | Weapon | +**30**% Movement Slow |
| Point Blank | 3,200 | Weapon | +**25**% Movement Slow |
| Weighted Shots | 3,200 | Weapon | +**30**% Movement Slow |
| Glass Cannon | 6,400 | Weapon | +**30**% Movement Slow |
| Haunting Shot | Legendary | Weapon | +**40**% Movement Slow |
| Lifestrike | 3,200 | Vitality | +**60**% Movement Slow |
| Majestic Leap | 3,200 | Vitality | +**40**% Movement Slow |
| Colossus | 6,400 | Vitality | +**30**% Movement Slow |
| Phantom Strike | 6,400 | Vitality | +**50**% Movement Slow |
| Cold Front | 1,600 | Spirit | +**60**% Movement Slow |
| Mystic Slow | 1,600 | Spirit | +**30**% Movement Slow |
| Slowing Hex | 1,600 | Spirit | +**20**% Movement Slow |
| Arctic Blast | 6,400 | Spirit | +**60**% Movement Slow |
| Lightning Scroll | 6,400 | Spirit | +**80**% Movement Slow |
| +**30**% Movement Slow |  |  |  |
| Mystic Reverb | 6,400 | Spirit | +**40**% Movement Slow |
| Vortex Web | 6,400 | Spirit | +**35**% Movement Slow |

### Movement Slow Resist

[edit | edit source]

#### Heroes

[edit | edit source]

| Hero | Ability | Slow Resistance |
| --- | --- | --- |
| Kelvin | Ice Path to self | 60% |
| Infernus | Flame Dash to self | 50% |

#### Items

[edit | edit source]

| Name | **** Cost | Category | Stat change |
| --- | --- | --- | --- |
| Fleetfoot | 1,600 | Weapon | +**35**% Movement Slow Resist (on use) |
| Enduring Speed | 1,600 | Vitality | +**25**% Movement Slow Resist |
| Juggernaut | 6,400 | Vitality | +**50**% Movement Slow Resist |

| | Stats |  | | --- | --- | | Weapon | Ammo •  Bullet Damage •  Bullet Velocity •  Damage per second •  Falloff Range •  Fire Rate •  Melee Damage •  Melee Distance •  Reload Time •  Weapon Damage | | Vitality | Bullet Evasion •  Damage Barrier •  Damage Resistance •  Debuff Resist •  Health •  Health Regen •  Healing •  Lifesteal •  Movement Slow •  Move Speed •  Slide Distance •  Stamina | | Spirit | Ability Cooldown •  Ability Duration •  Ability Range •  Bonus Ability Charges •  Imbue •  Spirit Damage •  Spirit Power •  Spirit Scaling | | Other | Abilities •  Build-Up •  Charge-Up •  Damage Amplification •  Hero Attributes Table •  Pure Damage •  Scaling •  Stack | |
| --- |