---
tags:
  - ults
  - combat
  - balancing
categoria: "[[08 - Cultures and Pantheons]]"
status: revised
---

# Divine Ult Rules

**Category:** [[08 - Cultures and Pantheons]]

Scale and shape rules for Divine Ultimates, common to all cultures. Each god offers **three ult paths** — Attack, Defense and Mobility — totaling **243 ults** in the system (81 gods × 3).

The ult is the fourth loadout slot described in [[3-Ability Combat System]]. The other three abilities come from profession; this one comes from the city's patron god.

## The Ult Belongs to the City, Not the Player

**The ult is tied to the deity, and the deity is tied to the city.** A player only has access to an ult while a citizen of a city whose patron deity grants it.

The ult **does not enter the [[Grimoire]]** and does not travel with the character. It is borrowed, not earned.

| Event | Effect |
|---|---|
| City advances an Era | The deity expires. All citizens lose the ult and gain access to the three of the new deity |
| City switches culture | Same, plus the Wrath of the Abandoned God on the city — see [[Deities and Passives]] |
| Player loses citizenship | Loses the ult immediately |
| Player migrates city | Gains the ults of the new city's deity |
| Nomad | Has no ult at all |

Since deities are era-locked, **no player keeps the same ult for more than one era**. The fourth slot is rotating by design.

## Core Principle

The number of units hit is **not defined by the era**. The target limit is determined by the area of effect (AoE) and by how many units stand inside it.

Era progression defines: presence or absence of AoE · maximum area size · effect intensity · duration · number of combined effects · strategic potential.

## Consolidated Scale

| Era | Maximum reach | Number of cells | Target type |
|---|---|---|---|
| Copper | No AoE | 1 target | One unit, building or object |
| Bronze | 3×3 | Up to 9 cells | All valid targets inside the area |
| Iron | 5×5 | Up to 25 cells | All valid targets inside the area |

The limit represents the **largest possible area**. Ults may use lines, crosses, cones, rings or smaller areas, as long as they fit within those dimensions.

### Copper Age — Single Target

Affects only one unit, hero, commander, building, object or a specific point of terrain, **without hitting the surrounding area**.

- Maximum area: 1 target.
- No area damage, healing or effect.
- The ability can be powerful against the chosen target.
- It cannot spread to nearby units nor create a zone affecting multiple units.
- Persistent effects must remain attached to the original target.

*Valid:* a divine arrow striking one enemy · a full heal on one ally · a shield on one unit · teleporting a character · protecting a building · a curse on a commander · repositioning a unit.

*Invalid:* an explosion hitting nearby units · circular healing · arrow rain · a barrier occupying several spaces · group teleport · a field granting bonuses to everyone inside it.

### Bronze Age — 3×3 AoE

- Maximum area: 3×3 cells (up to nine).
- Can be centered on a chosen cell.
- Can affect all valid units inside the area.
- Need not use all nine cells; smaller shapes are permitted.
- Can leave a temporary effect on the terrain.

**Permitted shapes:** full area · cross · line · short cone · ring.

**Expected intensity:** two moderate effects combined — damage and slow, healing and defense, teleport and speed, shield and counterattack, knockback and disorganization, camouflage and mobility.

### Iron Age — 5×5 AoE

- Maximum area: 5×5 cells (up to 25).
- Can affect large formations and multiple buildings.
- Can temporarily alter the terrain and create persistent zones.
- Can combine multiple effects, with different effects at center and edges.
- Can affect allies and enemies in distinct ways.

**Permitted shapes:** full area · extended cross · long line · cone · outer ring · **center and periphery** (epicenter with the strongest effect, inner area with normal effect, periphery with reduced effect).

**Expected intensity:** high damage · crowd control · terrain alteration · persistent penalty · ally bonuses · special effect at the epicenter · strategic effect after it ends.

## Power Progression Beyond Size

| | Copper | Bronze | Iron |
|---|---|---|---|
| Targets | One | Up to 3×3 | Up to 5×5 |
| Effects | One main effect | One strong or two moderate | Two or more relevant |
| Duration | Short or moderate | Moderate | Moderate or long |
| Terrain | — | Temporary effect | Terrain alteration |
| Impact | High individual intensity | Tactical control of a small area | Can decide an engagement |

## Rules by Category

### Mobility

- **Copper:** transports or accelerates only one target. Origin and destination have no AoE.
- **Bronze:** transports, accelerates or repositions all units in a 3×3 area. The destination area also respects 3×3. Units keep relative positions where possible.
- **Iron:** transports or repositions units from a 5×5 area. Can create a large-scale route or portal. Entry and exit respect 5×5. May ignore major obstacles according to the deity's theme.

### Defense

- **Copper:** protects one unit or building, possibly granting high individual resistance. Cannot generate an aura or area barrier.
- **Bronze:** protects up to 3×3. Shields, healing, camouflage or collective resistance. Can block narrow paths.
- **Iron:** protects up to 5×5. Can prevent destruction, alter terrain or create persistent zones. Can combine protection with healing, counterattack or control.

### Attack

- **Copper:** hits a single target, with high damage, control or a curse. **No collateral damage.**
- **Bronze:** hits up to 3×3, with damage and one secondary effect. Controls a small formation.
- **Iron:** hits up to 5×5, with damage, control and terrain alteration. May have a stronger epicenter and weaker edges, and leave persistent effects.

## Final Rule — Declaration Schema

Every ult must declare its reach in this format:

```yaml
era: copper | bronze | iron
category: attack | defense | mobility
target_type: unit | building | cell | area
aoe_shape: none | line | cross | cone | square | ring | custom
max_dimension:
  width: 1 | 3 | 5
  height: 1 | 3 | 5
affects:
  allies: true | false
  enemies: true | false
  buildings: true | false
duration: instant | temporary | persistent
```

Fixed constraints per era: Copper uses `aoe_shape: none` and dimension 1×1; Bronze, maximum dimension 3×3; Iron, 5×5.

## Mandatory Record per Ability

Because area size does not define a fixed number of people — a 3×3 ult may hit zero, one, nine or more units — each ability must separately record:

AoE shape · maximum dimension · valid targets · units per cell · line-of-sight requirement · interaction with obstacles · epicenter effect · edge effect · area duration.

## Open Questions

* Whether the **Wrath of the Abandoned God** leaves the city with no ult at all during the 24 hours, or whether the new deity delivers its ults immediately.
* Whether switching path (Attack to Defense, for example) within the same deity is free or carries a cost.
* What happens to a player who is outside the city, on caravan or expedition, at the moment the city turns an era and their ult expires.
* Cost, cooldown and activation condition of the ult — no document defines these.
* **Combat genre alignment.** These rules describe grid-based tactical combat with formations and commanders; [[3-Ability Combat System]] and [[Visual and Mechanical Direction]] describe precision action PvP with one character per player. The two readings still need reconciling.
