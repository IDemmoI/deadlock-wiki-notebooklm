# Heavy Melee

Overview

Heavy Melee Cancel

Heavy Melee Cancel Extension

Hidden Melee

| Heavy Melee |  |
| --- | --- |
| https://deadlock.wiki/File:Heavymelee.mp4 |  |
| Tech Type: | Universal Tech |
| Difficulty: | Basic Mechanics |
| Character Dependent: | No |
| Stamina: | 0 |
| Inputs: | Hold MeleeBy default,Q |

By pressing the melee key, you can execute a Light Melee. By holding the melee key, you can continue winding up your punch to execute a *Heavy Melee*. A full Heavy Melee lasts for 1.25 seconds and has a cooldown of 1.0 seconds when hit and 1.3 seconds when missed[1].

A Heavy Melee costs no stamina.

Heavy Melees are available both on the ground and in the air. There are three phases to a Heavy Melee: *windup*, *lunge* and *recovery*.[2]

## Contents

- 1 Windup
- 2 Lunge
- 3 Recovery
- 4 Items that increase Heavy Melee Distance

##### Windup

[edit | edit source]

Upon initiating a Heavy Melee, you enter the first phase: *windup*. During windup, you pull back and "windup" your punch. If you were on the ground upon initiation, you are instantly stopped while you windup.

During this phase, you are fully vulnerable and do not yet have a hitbox. While in windup, yellow and orange particle effects will be emitted from your fist and a noticeable sound effect will be played for all players. If you are in the air, you will continue in your current velocity, and be locked out of moving using the standard movement keys.

The windup phase takes 0.36 seconds.

##### Lunge

[edit | edit source]

After the windup phase is the *lunge* phase. During the lunge phase, you start lunging forwards and are able to damage other players. The peak speed at which you lunge is 750 u/s on the ground and 797 u/s in the air. With the  Weapon Item  Melee Charge, the peak speed is 1125 u/s on the ground and 1195 u/s while stationary in the air. With the upgrade,  Crushing Fists, the peak speed is 1200 u/s on the ground and 1275 u/s while stationary in the air.

During this phase, you have a hitbox attached to you. While you are moving, a small spherical hitbox is attached to your player which can damage opponents. Since you have a melee hitbox applied on your character, you are susceptible to being parried. If any enemy player is hit (including neutral creeps), the rest of the lunge phase is cancelled, the final hitbox will not appear and you immediately enter the recovery phase.

Visualisation of Heavy Melee using commands; the dense cluster is hitboxes while in the middle of lunge, the large cone and sphere are the final hitboxes.

While in lunge phase, turning is slightly restricted[3], with the maximum turn being ~300 degrees. Even with the restriction, you can still fake out opponents and take very sharp turns.

At the end of the lunge phase is a "final hit". This hitbox is much larger and is able to be aimed in any direction. This final hitbox consists of two checks:

- The game checks in a 192 unit sphere around you to check for enemy players (includes Neutral creeps and minions).
- The game checks in a conical frustum (200 units in length and 100 units in final radius) in front of your current position to check for enemy players (includes Neutral creeps and minions).
- If an enemies hurtbox is in both, they are hit and damaged.

While in the air, you are able to change your direction by ~5° upwards or downwards.

The damage that a Heavy Melee deals depends on the character; the normal damage amount is 116.  Ivy and  Yamato deal 116 and 128 melee damage, respectively, and  Paige deals 120 with *x*0.3 Spirit scaling. This damage can be increased by buying items that have the *+Melee Damage* stat or by buying items that increase Weapon Damage[4]

The lunge phase takes a maximum of 0.6 seconds.

##### Recovery

[edit | edit source]

After the lunge phase is the *recovery* phase. In this phase, you no longer have any active hitboxes and stand still. All previous momentum is cancelled and you stop at a standstill, both on the ground and in the air. If you are in the air, all momentum (both the x-axis and the y-axis) is cancelled for a moment.

The recovery phase takes 0.2833 seconds.

#### Items that increase Heavy Melee Distance

[edit | edit source]

Items with the *+Heavy Melee Distance* statistic increase the distance of a Heavy Melee. Examples include:

This is an automatic list. Click here to correct the contents.

| Name | ****Cost | Category | Stat change |
| --- | --- | --- | --- |
| Melee Charge | 1,600 | Weapon | +**50**% Heavy Melee Distance |
| Crushing Fists | 6,400 | Weapon | +**60**% Heavy Melee Distance |
| Runed Gauntlets | Legendary | Weapon | +**150**% Heavy Melee Distance |

1. ↑ abilities.data, EAttackType_Heavy; m_flCooldownOnHit, m_flCooldownOnMiss
1. ↑ Another way to think about it is like a standard move in a standard fighting game. A standard button has startup, active, and recovery frames
1. ↑ abilities.vdata, m_flHeavyMeleeMaxTurnRate. Implemented in 29 July, 2025 Update
1. ↑ Melee attack damage benefits from 50% of all Weapon Damage buffs.