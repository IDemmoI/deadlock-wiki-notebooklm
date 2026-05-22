# Souls

Soul released by the trooper.
Dark and light soul orb. Only light orbs can be claimed or denied

“

The more they die, the stronger I become!

— Graves

**Souls** are a crucial element in *Deadlock*, serving both as currency and experience points (XP) for heroes. Players collect souls by various means, including shooting **Soul Orbs** released when certain entities die, taking Guardians/Walkers, killing enemy players, and finding **Unsecured Souls** in boxes or crates. The amount of souls earned from a kill is a **Bounty**. Unsecured souls are added to your total immediately but can drop upon death for other players to collect.

Every player starts the game with  **600**.

## Contents

- 1 Soul Orbs

- 1.1 Local Soul Sharing
- 1.2 Soul Well
- 2 Gathering Souls

- 2.1 Soul Distribution
- 2.2 Denizens (Jungle Creeps)
- 2.3 Sinner's Sacrifices
- 2.4 Breakables
- 2.5 Other
- 3 Unsecured Souls
- 4 Leveling Up
- 5 Soul Values

- 5.1 First Blood bonus
- 5.2 Comeback Mechanics
- 5.3 Catch up Mechanics
- 6 Update history
- 7 References

## Soul Orbs

[edit | edit source]

Troopers and the Soul Urn release souls in **Soul Orbs**. These orbs may be shot or hit with melee to confirm (or deny) the souls and grant them to the attacker. If they are not attacked, then the souls will be granted to the killer automatically after around 1 second. Certain abilities like  Serrated Knives or  Malice can also confirm or deny orbs.

Troopers drop two orbs on death, one that floats and one that falls on the ground. The floating orb has 40% of the kill bounty and the ground orb has 60%. The ground orb cannot be denied (they appear as white to enemies) and remains for a few seconds before disappearing (their duration increases over time).

The floating soul orbs spawn dark-colored, and can only be shot and confirmed once they light up. Ally orbs are green and enemy orbs are orange. Hitting an enemy orb will deny the souls to the killer and grant them to the player who hit it. If the orb "pops" without being claimed, it's automatically rewarded to nearby allies, and if there are no allies nearby the souls are lost. Orbs can be claimed by a single bullet or pellet, regardless of damage. The bullet that hit the orb is refunded to the player's magazine.

Soul confirmation accounts for latency, which in some situations can cause the player to lose the orb even if they visually seem to have hit it first. The ally team has confirm advantage.

Soul orbs can be divided into "local" and "global" types:

Local
Orbs spawned by killing Troopers grant souls to the player who confirmed them and any nearby allies.
Global
Orbs spawned by delivering theSoul Urn grant souls to the entire team of the player who claims them.

### Local Soul Sharing

[edit | edit source]

When souls are to be shared, the game checks two distances to add allied heroes to the "pool" of heroes to split the received souls:

- 45m from the soul orb itself when it is broken
- 30m from the hero that killed the Trooper

If an allied hero is within **either** of these distances, souls are shared between the killer and those allied heroes.

### Soul Well

[edit | edit source]

Inside each team's base, there is a soul well that releases orbs worth 10 souls each. Unlike regular orbs, these orbs only grant souls if they are confirmed, and they can be either green or orange-colored.

## Gathering Souls

[edit | edit source]

- Teams with fewer souls will gain more souls from all sources (see ***Comeback Mechanics*** below).

### Soul Distribution

[edit | edit source]

- Hero kill souls are distributed between nearby players with the following rate:

- 125%/57%/28%/17%/11%/8% (for 1/2/3/4/5/6 players)

- EX: 1000 souls between 4 players would grant each player 170 souls (1000 * 17%)
- Additionally, for kills with two or more players, the player who got the kill receives bonus souls.
- Trooper souls are distributed between nearby players with the following rate:

- 100%/54%/36%/25%/20%/16% (for 1/2/3/4/5/6 players)

- EX: 120 souls between 4 players would grant each player 30 souls (120 * 25%)

- When a Trooper is killed, 60% of the Trooper's souls drop as a ground orb that flies to allies within 18m and remains on the ground for 18 seconds (scaling to 40 seconds after 10 minutes), while the remaining 40% fly out as a deniable soul orb that enemies can shoot. Both orbs use Soul distribution among nearby allies; enemy ground orbs are visible but cannot be claimed. Killing the Trooper with a melee attack grants 100% of the souls instantly, distributed among nearby allies.

### Denizens (Jungle Creeps)

[edit | edit source]

- Jungle camps contain Denizens that give souls to players on kill. They do not release soul orbs.

- In order for Denizens to give souls to both players, both players must deal damage to the Denizen.
- Souls from Denizens are split between all allied players who dealt damage to said Denizens.
- Souls from Denizens are **unsecured** souls.

### Sinner's Sacrifices

[edit | edit source]

- Some jungle camps contain one or two Sinner's Sacrifice machines, which grants souls to the player by hitting them with melee attacks. Those souls are unsecured.

### Breakables

[edit | edit source]

- Breaking the wooden crates scattered throughout the map will have a chance to spawn some souls.

- Chance for any given crate to drop souls when broken is approximately 60%
- Amount of souls dropped is a function of in-game time:

- *[Souls Dropped] = 23 + 2.0*[Game Time in Minutes]*
- For example: At 30:00 game time, a broken crate will drop 83 souls.

### Other

[edit | edit source]

- Trophy Collector is an item that gives the player passive souls per minute.

- Killing cockroaches in underground tunnels grants the player 1 soul each.

## Unsecured Souls

[edit | edit source]

Unsecured souls icon

Souls earned from killing Denizens and destroying Sinner's Sacrifice machines are **unsecured** and are lost on death. If a player dies with at least 150 unsecured souls they will be dropped in a **Soul Container**, which can be claimed by any player by hitting it with a Heavy Melee. Soul Containers will despawn after 3 minutes. These containers are marked with a circle icon on the Minimap and have a green glow effect. If a player dies with fewer than 150 unsecured souls, no Soul Container will drop—they are permanently lost.

Unsecured souls are converted into secured souls over time, meaning they will no longer be dropped on death. This conversion rate is dynamic:

- **Percentage Drain:** Each second, **0.5%** of the player's *current* unsecured souls are converted. This means larger amounts of unsecured souls secure faster initially.
- **Base Drain:** In addition to the percentage, a flat amount is secured every second. This starts at **1.6 souls/second** and increases as the match progresses (scaling with the global bounty growth of ~8% per minute).

- **Example at 10 Minutes:** A player carrying **1,000 unsecured souls** will secure them at a rate of roughly **7.9 souls/second** (5 from percentage + ~2.9 base).
- **Example at 20 Minutes:** That same player carrying **1,000 unsecured souls** will secure them faster, at a rate of roughly **9.2 souls/second** (5 from percentage + ~4.2 base), due to the base rate scaling over time.

Souls UI for Heroes

Unsecured souls may be spent in the shop, but are spent *after* secured souls. They are indicated by the silver-green ball on the Hero's hip known internally as a Soul Container, as well as in the number on the HUD with a red icon.

Unsecured souls count towards leveling up. However, if the player dies and loses those souls, they will remain at the last unlocked level but lose progress to the next level equivalent to their dropped souls.

On the character UI, the large souls number is the **total** number of secured and unsecured souls added together.

## Leveling Up

[edit | edit source]

Gathering souls will gradually "level up" your hero, granting a variety of benefits. See boons for detailed information.

## Soul Values

[edit | edit source]

- **Soul Value:** Value of the target at the time = 0m
- **Soul Gain:** How the value changes over the time of the match, measured in minutes

| Source | Soul Value | Combined Soul Gain (/min) |
| --- | --- | --- |
| Heroes | 250 | +48.75 |
| Trooper | 116 Total | +1.16 |
| Small Denizen | 41 | +0.44 |
| Medium Denizen | 68 | +0.73 |
| Large Denizen | 181 | +1.95 |
| Mid-Boss | 3000 | N/A |
| Sinner's Sacrifice | 310 | +3.35 |
| Soul Urn* | 1300 Total | +230 |
| Guardian** | 1500 | N/A |
| Walker** | 4000 | N/A |
| Base Guardian** | 1000 | N/A |
| Shrine | 2000 | N/A |
| Weakened Patron | 0 | N/A |
| Crates | 23 | +2.0 |

* Soul gain from Urns is divided among the team. The Courier gets slightly more souls.

** Soul gain from structures is split with 40% given to nearby allied heroes, while 60% is divided amongst the entire team.

### First Blood bonus

[edit | edit source]

- A player gets 150 bonus souls on their first kill.

### Comeback Mechanics

[edit | edit source]

When a team is behind on souls, there are some "comeback mechanics" that come into play to allow the losing team to quickly catch up.

- Killing an enemy hero will award more souls if that hero is stronger than the killer team's average networth, regardless of which team is leading in souls.
- The Soul Urn will give additional souls to the team that is behind based on game duration and total soul deficit. (see Soul Urn for details)
- The losing team gains up to 30% more souls from Troopers, Denizens, Sinner's Sacrifices and Objectives, based on how behind they are (peaks at 20% max net worth difference). The first 3k in net worth difference is ignored. (This means that the first 3k souls should be subtracted when calculating comeback values, e.g. 100k to 105k is calculated as a 2k difference)
- After 10 minutes in a match, killing a player whose net worth is above 15% higher than the killer team's average net worth increases that player's respawn time. The increase varies based on the net worth difference and match duration, from +6s for 15% net worth at 10 minutes to +22s for 30% net worth at 25 minutes.

### Catch up Mechanics

[edit | edit source]

Catch up mechanics allow for players with low net worth to catch up to the other players on their team.

- The two players per team with the lowest net worth have a passive gain of souls per second based on the total souls per second gathered by the team (2.5% and 1.5% for the lowest and second-lowest player, respectively). This occurs after laning phase (8 min).

- For example, if a team gathered 200 souls in the last second, the lowest player earns 5 extra souls.

## Update history

[edit | edit source]

*View the full update history: **Souls/Update history***

| Update | Changes |
| --- | --- |
| April 30, 2026 | - Souls required for boons after 13.2k/15k/17k/+2k per boon to 13.2k/14.5k/+1.5k per boon (ends at 40k instead of 49k) |
| December 16, 2025 | - Increased kill bounty for solo kills (1 attacker in the kill) by 25%, and by 15% for duo kills - Increased portion of the bounty the killer gets relative to the assist portion - Increased comeback bounties for losing team a bit - Unsecured souls claim period reworked. Previously the way it worked was any unsecured souls you gained were added to a rolling 165s window, where it was divided over that time and given out, with a minimum amount given per second of 1 soul. The new system drains 0.5% (of the remaining souls) + 1.6 (scales with the 8% bounty growth per minute).   - - There are a few examples below to show how they compare. Old was 165s (assuming bounty was at least 165s). New is:   - - - 1x Small Camp: 77s - 2x Medium Camps: 163s - 1x Hard Camp: 193s - 4x Medium Camps: 230s - 2x Hard Camps: 263s - 1x Hard Camp + 3x Medium Camps: 270s - 2x Hard Camp + 6x Medium Camps: 354s |
| November 23, 2025 | - Hero kill bounty split efficiency for 1/2/3/4/5/6 players changed from 100/100/90/84/65/72% to 100/100/85/70/55/50% |

## References

[edit | edit source]

| | Gameplay |  | | --- | --- | | General | Abilities • Glossary • Heroes • Hideout • Items • Map • Skill Rating • Stats • Strategy • Street Brawl | | Map features | Cosmic Veil • Crate • The Curiosity Shop • Golden Statue • Jump pad • Mid-Boss • Neutrals • Powerup • Rejuvenator • Ropes • Sinner's Sacrifice • Soul Urn • Structures • Teleporter • Vent • Ziplines | | Mechanics | Backdoor Protection • Boon • Cheater Frog • Crowd Control • Death • Extra Slots • Health • Melee Attack • Minimap • Movement • Souls • Stack • Status Effects | |
| --- |