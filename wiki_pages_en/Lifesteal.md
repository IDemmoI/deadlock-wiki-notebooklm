# Lifesteal

**Lifesteal** is a mechanic which heals a player by a portion of the damage they deal to an opponent. There are two main types of lifesteal, each with an associated stat:  Bullet Lifesteal, which returns a portion of the bullet damage dealt, and  Spirit Lifesteal, which returns a portion of the spirit damage dealt. Bullet and Spirit Lifesteal are calculated independently, but use the same formula.

## Contents

- 1 Calculation

- 1.1 Example
- 1.2 Lifesteal vs. Creeps
- 2 Bullet Lifesteal

- 2.1 Sources
- 2.2 Hero Abilities
- 3 Spirit Lifesteal

- 3.1 Sources
- 3.2 Soul Shredder Bullets
- 4 Melee Lifesteal

## Calculation

[edit | edit source]

While lifesteal is shown as a percentage (like +20%), different sources of lifesteal do not simply add together. Instead, they stack **multiplicatively**. This means that as you gain more sources of lifesteal, each new item is slightly less effective than the last.

To calculate your final lifesteal, you can use the following formula:

Total Lifesteal=1−(1−L1)×(1−L2)×(1−L3)…

(Where L is the lifesteal value of each source expressed as a decimal, e.g., 0.20 for 20%).

### Example

[edit | edit source]

If you have 22% Bullet Lifesteal from  Fury Trance and 30% Bullet Lifesteal from  Leech, your lifesteal is calculated as follows:

1. Convert the percentages to decimals: **0.22** and **0.30**.
1. Subtract each from 1: (1 - 0.22) = **0.78** and (1 - 0.30) = **0.70**.
1. Multiply those results together: 0.78 × 0.70 = **0.546**.
1. Subtract that result from 1: 1 - 0.546 = **0.454**.
1. Your final Bullet Lifesteal is **45.4%**.

Note: The in-game user interface is inconsistent with rounding, so it may display as 45% or 46%.

### Lifesteal vs. Creeps

[edit | edit source]

Lifesteal against creeps (non-hero units) is reduced compared to heroes:

- **Bullet Lifesteal vs. creeps:** 60% effectiveness (e.g., 10% lifesteal becomes 6%).
- **Spirit Lifesteal vs. creeps:** 40% effectiveness (e.g., 10% lifesteal becomes 4%).

## Bullet Lifesteal

[edit | edit source]

Bullet Lifesteal returns a percentage of all outgoing bullet damage to the player as health.

Graves has 8% innate Bullet Lifesteal.

### Sources

[edit | edit source]

This is an automatic list. Click here to correct the contents.

| Name | ****Cost | Category | Stat change |
| --- | --- | --- | --- |
| Active Reload | 1,600 | Weapon | +**14**% Bullet Lifesteal |
| Bullet Lifesteal | 1,600 | Vitality | +**13**% Bullet Lifesteal |
| Fury Trance | 3,200 | Vitality | +**14**% Bullet Lifesteal |
| Leech | 6,400 | Vitality | +**25**% Bullet Lifesteal |
| Vampiric Burst | 6,400 | Vitality | +**13**% Bullet Lifesteal |
| +**70**% Bullet Lifesteal |  |  |  |

### Hero Abilities

[edit | edit source]

Abilities that deal weapon damage also provide heal from Bullet Lifesteal. Here are all of the relevant abilities.

This is an automatic list. Click here to add notes or correct the contents.

| Hero | Ability |
| --- | --- |
| Bebop | Exploding Uppercut |
| Bebop | Grapple Arm |
| Billy | Bashdown |
| Calico | Leaping Slash |
| Drifter | Rend |
| Silver | Boot Kick |
| Silver (Transformed) | Go For The Throat |
| Silver (Transformed) | Mauling Leap |
| Venator | Consecrating Grenade |
| Venator | Gutshot |
| Venator | Ira Domini |
| Viscous | Puddle Punch |
| Yamato | Flying Slash |

## Spirit Lifesteal

[edit | edit source]

Spirit Lifesteal returns a percentage of all outgoing spirit damage to the player as health.

### Sources

[edit | edit source]

This is an automatic list. Click here to correct the contents.

| Name | ****Cost | Category | Stat change |
| --- | --- | --- | --- |
| Spirit Shredder Bullets | 1,600 | Weapon | +**10**% Spirit Lifesteal |
| Spirit Rend | 3,200 | Weapon | +**10**% Spirit Lifesteal |
| Spiritual Overflow | 6,400 | Weapon | +**16**% Spirit Lifesteal |
| Spirit Lifesteal | 1,600 | Vitality | +**13**% Spirit Lifesteal |
| Infuser | 6,400 | Vitality | +**70**% Spirit Lifesteal |
| Leech | 6,400 | Vitality | +**25**% Spirit Lifesteal |
| Mystic Reverb | 6,400 | Spirit | +**8**% Spirit Lifesteal |

### Soul Shredder Bullets

[edit | edit source]

The debuff applied to opponents by  Spirit Shredder Bullets behaves differently from all other lifesteal items. It does not affect the user's Spirit Lifesteal stat, nor is it factored into the multiplicative formula; instead, it **adds** a flat +10% spirit lifesteal against an affected target while the debuff is active.

For example, if a player has Spirit Lifesteal (+16%) and  Leech (+30%), their base spirit lifesteal is 41.2%. Against a target affected by Soul Shredder Bullets, it would be:

Total Lifesteal=[1−(1−0.16)×(1−0.30)]+0.1=51.2%

## Melee Lifesteal

[edit | edit source]

Main articles: Melee Lifesteal, Lifestrike

Melee Lifesteal is not a stat. The item  Melee Lifesteal and its upgrade  Lifestrike both provide a passive ability which heals the user by a percentage of their melee damage dealt, but they behave differently from Bullet and Spirit Lifesteal.

These abilities activate for one melee attack, then go on cooldown for several seconds, during which no further health can be regained from melee attacks. In contrast, Bullet and Spirit Lifesteal are always active and have no cooldowns. These items also grant a flat healing bonus on activation, and are less effective against non-heroes.

| | Stats |  | | --- | --- | | Weapon | Ammo •  Bullet Damage •  Bullet Velocity •  Damage per second •  Falloff Range •  Fire Rate •  Melee Damage •  Melee Distance •  Reload Time •  Weapon Damage | | Vitality | Bullet Evasion •  Damage Barrier •  Damage Resistance •  Debuff Resist •  Health •  Health Regen •  Healing •  Lifesteal •  Movement Slow •  Move Speed •  Slide Distance •  Stamina | | Spirit | Ability Cooldown •  Ability Duration •  Ability Range •  Bonus Ability Charges •  Imbue •  Spirit Damage •  Spirit Power •  Spirit Scaling | | Other | Abilities •  Build-Up •  Charge-Up •  Damage Amplification •  Hero Attributes Table •  Pure Damage •  Scaling •  Stack | |
| --- |