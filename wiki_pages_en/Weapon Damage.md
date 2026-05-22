# Weapon Damage

**Weapon Damage** is a stat that determines the player's Bullet Damage, and also increases their Melee Damage. Some abilities can deal Weapon Damage.

Load video

YouTube

YouTube might collect personal data. Privacy Policy

Continue
Dismiss

Video explaining Weapon Damage

## Contents

- 1 Base Weapon Properties

- 1.1 Base Bullet Damage
- 1.2 Spreadshots
- 1.3 Piercing shots
- 1.4 Melee Damage
- 2 Combat Modifiers

- 2.1 Damage Falloff
- 2.2 Crit Multiplier
- 3 Target Modifiers

- 3.1 Bullet Resistance
- 3.2 Increased Bullet Damage
- 4 Flat Weapon Damage
- 5 Weapon Damage Formula
- 6 Weapon Damage Scaling
- 7 Sources
- 8 References

## Base Weapon Properties

[edit | edit source]

### Base Bullet Damage

[edit | edit source]

Base Bullet Damage is the amount of damage your Hero deals with no items. This value is unique to each hero and increases automatically as you level up through Boons.

### Spreadshots

[edit | edit source]

Spreadshots allow certain weapons to fire multiple bullets at once (such as shotguns or shurikens). In these cases, all calculation rules apply to every individual bullet.

### Piercing shots

[edit | edit source]

Paige's weapon's shots pierce through enemies and can hit multiple enemies per projectile, disappearing only when they hit a map surface. However, they do not deal headshot bonus damage, but can proc headshot items.

The Doorman's weapon's shots also pierce enemies. Unlike Paige's, they can deal headshot damage but deal half damage to all enemies hit after the first.

### Melee Damage

[edit | edit source]

Melee Damage scales with Weapon Damage by 50%. However, Melee Damage is *not* considered Weapon Damage, thus effects that block Weapon Damage such as  Metal Skin have no effect against melee unless noted otherwise.

## Combat Modifiers

[edit | edit source]

### Damage Falloff

[edit | edit source]

Damage Falloff reduces damage based on distance. All heroes have a Falloff Range in which damage is linearly reduced from 100% to 10%.

When aiming at an enemy hero, a dot on their health bar indicates the percentage of damage you will deal:

| Dot Color | Damage Percentage |
| --- | --- |
| **Red** | 10% - 20% |
| **Orange** | 20% - 35% |
| **Yellow** | 35% - 75% |
| **Transparent** | 75% - 100% |

### Crit Multiplier

[edit | edit source]

Aiming for the head deals increased damage. Troopers, Guardians, and Heroes have a weakpoint hitbox that receives **1.65x** bullet damage when hit.

Crit Multiplier=[1+(0.65×Crit Bonus Scale)]×Crit Resist

The following heroes cannot deal critical damage:

- Graves
- Paige (though she can proc headshot item effects)

**Crit Bonus Scale** is a stat that modifies critical damage for certain heroes.

| Hero | Crit Bonus Scale (%) |
| --- | --- |
| Billy | -20 |
| Celeste | -25 |
| The Doorman | -25 |
| Drifter | -45 |
| Kelvin | -25 |
| Rem | -20 |
| Vyper | -30 |

Abilities that can deal critical damage have different critical modifiers. This replaces the +65% multiplier of base weapons.

| Hero | Ability | Crit Damage (%) |
| --- | --- | --- |
| Paradox | Kinetic Carbine | 14 |
| Venator | Ira Domini | 30 |
| Vindicta | Assassinate | 20 |

## Target Modifiers

[edit | edit source]

### Bullet Resistance

[edit | edit source]

Main article: Damage Resistance

Incoming damage is reduced by the target's **Bullet Resist** and increased by the attacker's **Bullet Resist Reduction**. These stats stack multiplicatively. For a detailed breakdown on how multiple items stack, see the main page.

### Increased Bullet Damage

[edit | edit source]

Increased Bullet Damage is a debuff inflicted on enemies. It multiplies the total amount of damage they take from you. Because this is applied at the end of the calculation, it also increases the effectiveness of your Flat Weapon Damage.

## Flat Weapon Damage

[edit | edit source]

Flat Weapon Damage is an extra amount of damage obtained through certain hero abilities.

**Flat Weapon Damage is not increased by your "Weapon Damage %" multiplier.** It is an additive source added to your total *after* the percentage multiplier is applied to your base. However, it is still affected by Damage Falloff, Bullet Resist, and Crit Multipliers.

## Weapon Damage Formula

[edit | edit source]

The final damage dealt by a bullet is determined by multiplying your base stats, your item bonuses, and various situational modifiers.

Final Damage=[(Base Damage×Weapon Damage Multiplier)+Flat Bonus]×Falloff×Resistances×Crit Multiplier

## Weapon Damage Scaling

[edit | edit source]

Some abilities scale with Weapon Damage.

For most Weapon Damage scaling abilities, they only scale based on the "Bonus Weapon Damage" stat, which is granted by items and Weapon shop investments (see list below). This includes abilities such as  Venator's  Consecrating Grenade,  Gutshot and  Ira Domini.  Paradox's  Kinetic Carbine is an exception, since it scales with her Base Weapon Damage (counting as a full burst shot), and thus increases with Boons. Melee Damage scaling abilities also scale with Weapon Damage, since Melee Damage scales with Weapon Damage (by 50%).

## Sources

[edit | edit source]

All weapon items provide an automatic increase in Weapon Damage based on the player's total soul investment in that category:

| Souls invested | Weapon Damage Increase |
| --- | --- |
| **800** | +9% |
| **1,600** | +12% |
| **2,400** | +15% |
| **3,200** | +18% |
| **4,800** | **+46%** |
| **7,200** | +55% |
| **9,600** | +70% |
| **16,000** | +85% |
| **22,400** | +100% |
| **28,800** | +115% |

The following items grant increased weapon damage:

This is an automatic list. Click here to correct the contents.

| Name | ****Cost | Category | Stat change |
| --- | --- | --- | --- |
| Close Quarters | 800 | Weapon | +**20**% Weapon Damage |
| Extended Magazine | 800 | Weapon | +**8**% Weapon Damage |
| High-Velocity Rounds | 800 | Weapon | +**8**% Weapon Damage |
| Restorative Shot | 800 | Weapon | +**6**% Weapon Damage |
| Long Range | 1,600 | Weapon | +**40**% Weapon Damage |
| Opening Rounds | 1,600 | Weapon | +**8**% Weapon Damage |
| Recharging Rush | 1,600 | Weapon | +**10**% Weapon Damage |
| Slowing Bullets | 1,600 | Weapon | +**15**% Weapon Damage |
| Titanic Magazine | 1,600 | Weapon | +**14**% Weapon Damage |
| Cultist Sacrifice | 3,200 | Weapon | +**8**% Weapon Damage |
| Escalating Resilience | 3,200 | Weapon | +**15**% Weapon Damage |
| Express Shot | 3,200 | Weapon | +**8**% Weapon Damage |
| Headhunter | 3,200 | Weapon | +**5**% Weapon Damage |
| Hollow Point | 3,200 | Weapon | +**35**% Weapon Damage |
| Point Blank | 3,200 | Weapon | +**50**% Weapon Damage |
| Sharpshooter | 3,200 | Weapon | +**70**% Weapon Damage |
| Weighted Shots | 3,200 | Weapon | +**40**% Weapon Damage |
| Armor Piercing Rounds | 6,400 | Weapon | +**8**% Weapon Damage |
| Glass Cannon | 6,400 | Weapon | +**80**% Weapon Damage |
| Battle Vest | 1,600 | Vitality | +**15**% Weapon Damage |
| Colossus | 6,400 | Vitality | +**15**% Weapon Damage |
| Inhibitor | 6,400 | Vitality | +**10**% Weapon Damage |
| Leech | 6,400 | Vitality | +**12**% Weapon Damage |
| Phantom Strike | 6,400 | Vitality | +**15**% Weapon Damage |
| Siphon Bullets | 6,400 | Vitality | +**15**% Weapon Damage |
| Unstable Concoction | Legendary | Spirit | +**150**% Weapon Damage |

- Headshot Booster deals +45 bonus Weapon Damage with headshots.
- Monster Rounds increases Weapon Damage against NPCs by +25%.
- Berserker increases Weapon Damage by +7% per stack for sustaining damage.
- Headhunter additionally deals +75 *x*4 bonus Weapon Damage with headshots.
- Intensifying Magazine increases Weapon Damage to a maximum of 45% after continuously firing.
- Opening Rounds increases Weapon Damage by +30% against enemies above 50% health.

## References

[edit | edit source]

| | Stats |  | | --- | --- | | Weapon | Ammo •  Bullet Damage •  Bullet Velocity •  Damage per second •  Falloff Range •  Fire Rate •  Melee Damage •  Melee Distance •  Reload Time •  Weapon Damage | | Vitality | Bullet Evasion •  Damage Barrier •  Damage Resistance •  Debuff Resist •  Health •  Health Regen •  Healing •  Lifesteal •  Movement Slow •  Move Speed •  Slide Distance •  Stamina | | Spirit | Ability Cooldown •  Ability Duration •  Ability Range •  Bonus Ability Charges •  Imbue •  Spirit Damage •  Spirit Power •  Spirit Scaling | | Other | Abilities •  Build-Up •  Charge-Up •  Damage Amplification •  Hero Attributes Table •  Pure Damage •  Scaling •  Stack | |
| --- |