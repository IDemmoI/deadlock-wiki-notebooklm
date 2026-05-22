# Dashing

Overview

Strafe Dashing

Dash Jumping

Dash Sliding

Short Dash Crouch Cancelling

Instant Air Dash

Ag2 Dashing

| Dashing |  |
| --- | --- |
| Load video     Local File     Local File might collect personal data.     Continue Dismiss  https://deadlock.wiki/File:Dashing.mp4 |  |
| Tech Type: | Universal Tech |
| Difficulty: | Basic Mechanics |
| Character Dependent: | No |
| Inputs: | DashBy default, the left shift key |

**Dashing** is a fundamental part of movement in Deadlock. Dashing allows you to quickly evade attacks, to reposition fast and efficiently, and is a basic building block for other basic and advanced movement techniques.

Dashing takes one bar of stamina. You can dash both in the air and on the ground; when done in the air, it is called an **Air Dash**. You are only permitted one Air Dash per jump at the start of the game; this can be expanded to two with the  Vitality Item  Stamina Mastery.

Using a keyboard, you can dash in four directions on the ground (the four cardinal directions) and nine in the air (the eight inter-cardinal directions plus directly down). If you are using a joystick to move, you can dash at any angle on the ground and in the air.

While in the air, you have access to one other direction to dash to; down towards the ground. When you dash towards the ground, it is called a **Down dash**. To down dash, double tap the duck key; once you press the duck key, you have a *28 ticks* (*0.44* second) window to press it again.[1]

Dash choices on the ground.

*0.3* seconds after starting a grounded dash, a window to execute a Dash Jump will open for *0.2* seconds,[2] during which the stamina bar flashes a light blue. This window is solely activated by starting a grounded dash; if you leave the ground after initiating the dash, you are still able to dash. For more information, view the dedicated page on Dash Jumping.

While everyone in the roster has the same dash distance, they have different dash speeds. Characters fall into three **buckets**[3]:

- **Bucket 1** characters have the fastest dash speed, with peak speeds of *635* u/s on the ground and a total dash time of *0.62* seconds.[4]
- **Bucket 2** characters have 9% slower dash speed, with peak speeds of *579* u/s on the ground and a total dash time of *0.68* seconds.[5]
- **Bucket 3** characters have the slowest dash speed, being 12% slower than Bucket 1, with peak speeds of *562* u/s on the ground and a total dash time of *0.70* seconds.[6]

Dashing on the ground always sets your velocity to a fixed amount. Air Dashing is an *impulse* instead, meaning it can stack or conflict with prior momentum.

Dash choices in the air.

To dash, move and press the dash keyBy default, the left shift key. Your character will quickly move in that direction.

##### Dash Speed Character Buckets

[edit | edit source]

| Bucket 1 | Bucket 2 | Bucket 3 |
| --- | --- | --- |
| Calico | Apollo | Abrams |
| Celeste | Billy | Bebop |
| Grey Talon | Drifter | Dynamo |
| Haze | Graves | Kelvin |
| Holliday | Infernus | Lady Geist |
| Ivy | Lash | Mo & Krill |
| Mina | McGinnis | Paige |
| Paradox | Mirage | Shiv |
| The Doorman | Pocket | Venator |
|  | Rem | Victor |
|  | Seven |  |
|  | Silver |  |
|  | Silver (Transformed) |  |
|  | Sinclair |  |
|  | Vindicta |  |
|  | Viscous |  |
|  | Vyper |  |
|  | Warden |  |
|  | Wraith |  |
|  | Yamato |  |

#### Abilities that decrease dash speed

[edit | edit source]

This is an automatic list. Click here to add notes or correct the contents.

| Hero | Ability | Dash Slow | Notes |
| --- | --- | --- | --- |
| Bebop | Hyper Beam | 40% | — |
| Celeste | Shining Wonder | 25% | T1 upgrade increases dash slow by 15% (total 40%). |
| Haze | Sleep Dagger | 50% (T3) | — |
| Kelvin | Arctic Beam | 20% | — |
| McGinnis | Heavy Barrage | 30% (T1) | Gives 35% dash slow for the caster. |
| Mo & Krill | Sand Blast | 25% (T2) | — |
| Rem | Naptime | 25% | — |
| Victor | Aura of Suffering | 25% (T1) | — |
| Victor | Shocking Reanimation | 30% | — |

##### Items that increase/decrease dash distance

[edit | edit source]

This is an automatic list. Click here to correct the contents.

| Name | ****Cost | Category | Stat change |
| --- | --- | --- | --- |
| Slowing Bullets | 1,600 | Weapon | -**25**% Dash distance |
| Weighted Shots | 3,200 | Weapon | -**25**% Dash distance |
| Haunting Shot | Legendary | Weapon | -**40**% Dash distance |
| Metal Skin | 3,200 | Vitality | -**20**% Dash distance |
| Stamina Mastery | 3,200 | Vitality | +**23**% Dash distance |
| Colossus | 6,400 | Vitality | -**25**% Dash distance |
| Mystic Slow | 1,600 | Spirit | -**12**% Dash distance |
| Slowing Hex | 1,600 | Spirit | -**30**% Dash distance |
| Lightning Scroll | 6,400 | Spirit | -**12**% Dash distance |
| Vortex Web | 6,400 | Spirit | -**40**% Dash distance |

1. ↑ Tested using exec_async, using the amount of space between +duck inputs.
1. ↑ abilites.vdata, m_flDashJumpStartTime and m_flDashJumpEndTime
1. ↑ Buckets is the official terminology used by Yoshi. Source: July 29, 2025 Update
1. ↑ heroes.vdata, hero_tengu, EGroundDashDuration = 0.620000. This is the same for all Bucket 1 characters.
1. ↑ heroes.vdata, hero_gigawatt, EGroundDashDuration = 0.680000. This is the same for all Bucket 2 characters.
1. ↑ heroes.vdata, hero_shiv, EGroundDashDuration = 0.700000. This is the same for all Bucket 3 characters.