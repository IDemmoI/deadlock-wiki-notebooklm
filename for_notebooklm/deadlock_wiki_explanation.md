# Deadlock Wiki Ingestion Guide and Formatting Explanation

This document provides critical context and explanations of the formatting, structures, and math syntax used in the consolidated Deadlock Wiki Markdown files (`deadlock_wiki_english_part1.md` through `part4.md`). NotebookLM must use this guide to correctly interpret hero stats, weapon parameters, ability cards, spirit scaling, and item upgrades.

---

## 1. Hero Base Stats Tables
On each Hero's page, base statistics are represented in Markdown tables under the **BASE STATS** heading.
Example:
```markdown
| | Damage Per Second: | 48.7 | | --- | --- | | Bullet Damage: | 18.5+0.825 |
```
*   **Stat Growth Per Level (The `Base+Growth` Syntax)**: Values formatted with a plus sign (e.g., `18.5+0.825`) indicate that the base value is `18.5` at Level 1, and it increases by `0.825` for each hero level gained.
*   **Weapon Stats**: Includes Damage Per Second, Bullet Damage, Ammo, Bullets per sec, Reload Time, Bullet Velocity, Light Melee damage, Heavy Melee damage, and Falloff Range.
*   **Vitality Stats**: Includes Health, Health Regen, Move Speed, Sprint Speed, Dash Speed, Stamina, and Stamina Cooldown.
*   **Spirit Power Stats**: Shows the base Spirit Power and Spirit Power growth (e.g., `0+1.1`).

---

## 2. Ability Cards & Spirit Power Scaling
Each Hero has an **Abilities** section. Below each ability name, there is a vertical text block representing the in-game ability card.

### Spirit Power Scaling (The `*x*Multiplier` Syntax)
*   **Definition**: Any multiplier formatted as `*x*Multiplier` or `xMultiplier` (e.g., `*x*1.3`, `*x*0.55`) represents the **Spirit Power Scaling Factor** (Spirit Scaling) for the stat immediately following or preceding it.
*   **Formula**: `Total Stat Value = Base Value + (Scaling Factor * Hero's Current Spirit Power)`.
*   **Example 1**:
    ```markdown
    *x*1.3
    **85**
    Damage
    ```
    *   **Interpretation**: The ability has a **Base Damage of 85**. The damage scales with Spirit Power by a factor of **1.3**.
    *   *Calculation*: If the hero has 50 Spirit Power, the actual damage dealt will be: `85 + (1.3 * 50) = 85 + 65 = 150`.
*   **Example 2**:
    ```markdown
    *x*0.55
    **25**
    Base Damage
    ```
    *   **Interpretation**: The ability has a **Base Damage of 25**, scaling with Spirit Power by a factor of **0.55**.

### Cooldown and Charges
*   **Cooldown**: A time value like `12s` or `26s` directly below the ability title indicates the base cooldown of that ability.
*   **Charges**: Indicates the maximum number of charges and the recharge time per charge if the ability is charge-based.

### Ability Upgrades (Tiers 1, 2, and 3)
In Deadlock, abilities are upgraded using Ability Points (AP). In the markdown files, upgrades are represented by bold numbers:
*   **1** corresponds to **Tier 1 Upgrade** (costs 1 AP).
*   **2** corresponds to **Tier 2 Upgrade** (costs 2 AP).
*   **5** corresponds to **Tier 3 Upgrade** (costs 5 AP).
*   **Upgrade Bonuses**: The text directly following the tier number explains the upgrade bonus.
    *   *Example*:
        ```markdown
        **1**
        -7s Cooldown
        **2**
        30% Melee Resist
        **5**
        1.6s Stun Duration
        ```
        *   **Interpretation**: 
            *   Tier 1 upgrade reduces the cooldown by 7 seconds.
            *   Tier 2 upgrade adds 30% Melee Resistance.
            *   Tier 3 upgrade increases the stun duration to 1.6 seconds.

---

## 3. Items and Shop Stats
On Item pages, statistics and prices are represented in tables like:
```markdown
| Name | ****Cost | Category | Stat change |
| --- | --- | --- | --- |
| Spellslinger | 6,400 | Weapon | +6% Ability Cooldown Reduction |
```
*   **Category**: Items belong to one of three categories: **Weapon** (Orange/Red), **Vitality** (Green), or **Spirit** (Purple).
*   **Cost**: The cost in Souls required to purchase the item (e.g., `500`, `1,250`, `3,000`, `6,200`).
*   **Stat changes**: Shows passive stats gained from buying the item (e.g., `+6% Ability Cooldown Reduction`).
