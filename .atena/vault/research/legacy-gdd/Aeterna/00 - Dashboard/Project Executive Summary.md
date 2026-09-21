---
tags:
  - dashboard
  - executive-summary
  - project
  - gdd
  - aetherna
categoria: "[[00 - Dashboard]]"
status: approved
---

# Project Executive Summary

## Overview

**Aetherna** is a hardcore Open Source sandbox MMO in **stylized painterly 3D**, with a player-run economy, emergent urban politics, physical transport of resources, high-risk PvP and seasonal progression closed out by [[Hard Wipe]] cycles.

The playable client is free. Creating content requires [[Editor Mode]] (R$ 10.00, one-time payment). Mods are open. Authored content circulates through the [[Lore Market]], where the game retains 10% of sales. There is no other monetization. The [[Official Server]] is out of scope.

The project is structured for iterative development with AI, using modular documentation in Obsidian and a future monorepo technical base with clean architecture, strong typing and an authoritative server distributed with the code and hosted by the community.

## Core Premise

Aetherna starts from a simple premise: *everything that matters must exist in the world.*

Resources must be gathered, items must be forged, letters must be carried, cities must be defended, and political power must be sustained by logistics, economy and risk.

The player does not progress mainly by level. They progress through knowledge, reputation, territory, alliances, economic dominance, mechanical skill and seasonal memory.

## Design Pillars

1. **Materiality** — no good, message or advantage exists outside the simulated physical world. If something must travel from A to B, someone carries it.
2. **Permanent risk** — Full Loot in the open world. Every journey is a gamble.
3. **Emergent, temporary power** — cities, offices, monopolies and borders are created by players and destroyed by the Cataclysm.
4. **Information as a scarce resource** — communication is limited by geography and by language; intercepting a letter is an act of war.
5. **Skill above capital** — item quality comes from precision minigames; combat comes from action skill; reputation comes from work.
6. **Impermanence with memory** — the wipe erases wealth, never identity: the Grimoire, titles and relics survive.

---

## 01 - Core Loop

The player's initial cycle runs from Nomad to Citizen.

- [[The Nomad Phase]]
- [[Gathering and Minigames System]]

Key decisions:

- Players are born at random locations far from cities.
- The open world carries the risk of Full Loot.
- Stamina limits movement, gathering, combat and transport.
- The game has no fixed classes.
- The player builds a loadout with 3 basic profession abilities and 1 divine ultimate.
- Unlocked profession abilities enter the permanent Grimoire.
- Gathering and crafting use proficiency minigames.
- Items can be Common, Refined or Masterpiece quality.

## 02 - Political and Urban System

Cities are political entities founded, governed and contested by players.

- [[The Town Hall and the Council]]
- [[War and Expansion Policy]]
- [[Repossession and Land Plots]]
- [[Urban Zoning and Elite Zones]]
- [[Communication and Espionage System]]
- [[Languages and Letter Security]]

Key decisions:

- **Five houses close together in a habitable zone unlock the Gathering Point.** Building it is what founds the city and chooses its Descent.
- In the Stone Age, decisions are made by **in-person voting** — the orality of the era.
- **Each culture has its own structure of government.** There is no single political model.
- **Writing is a political advantage.** Cultures with writing replace in-person voting with recorded voting and govern at a distance; oral cultures cannot, but are immune to record destruction.
- The governing body administers taxes, wars, laws, urban development and the choice of patron deity.
- Cities can conquer and annex other cities.
- Defeated players enter the Trial Stage.
- Text chat exists only within urban borders.
- In the open world, communication is limited to proximity VoIP.
- Diplomacy between cities requires a physical Letter carried by Emissaries.
- Languages function as cultural encryption.

## 03 - Economy and Market

The economy is local, physical and vulnerable to inflation, theft, war and political decision.

- [[Open Source Model and Monetization]]
- [[The Tax and Gold System]]

Key decisions:

- There is no global auction house.
- Each city has a local market.
- Arbitrage depends on [[Caravan Logistics]].
- The Council sets the local market tax.
- Faucets include ore, trees, hunting, chests and exploration.
- Sinks include durability, repairs, taxes, urban upkeep and temple offerings.
- **Tax revenue goes entirely to the public treasury. The game takes no share.**
- Monetization follows the Zero Pay-to-Win rule.
- **The VIP system and monthly subscription have been discontinued.**
- The Mobile Base remains a mechanic, unlockable in-match, and remains vulnerable.

## 04 - Logistics and Open World

The map is an economic, military and political system in itself.

- [[Caravan Logistics]]

Key decisions:

- The world uses a continuous map with **vertical terrain** — height is a game rule, not decoration.
- There are no invisible walls or loading screens between biomes.
- Main trails offer speed and lower stamina cost, but increase exposure.
- Off-road offers stealth, but reduces speed and drains stamina.
- Biome transition zones are natural ambush points.
- There is no Fast Travel.
- Every resource must be physically transported.
- Cargo weight affects caravan speed and risk.
- PvE acts as an ecological toll and war of attrition before PvP.

## 05 - Combat and Factions

Combat is **precision action PvP**: positioning, range, execution timing, stamina and reading intent.

- [[3-Ability Combat System]]
- [[Bandits and Full Loot]]
- [[Death and Respawn Dynamics]]

Key decisions:

- Dying in the open world drops the inventory on the ground.
- Respawn carries a cumulative penalty to prevent the zombie tactic.
- Nomads respawn randomly in the world.
- Citizens respawn in their house bed.
- There are no fixed global factions.
- Criminal fame emerges from player actions.
- Cities can issue Bounties using municipal treasury gold.
- Bandits can build Clandestine Camps in the Fog of War.
- **The divine ult belongs to the city, not the player.** Losing citizenship costs the ult.

## 06 - Seasons and Lore

Aetherna is a seasonal world, made to be born, grow, collapse and be reborn.

- [[Seasons and Hard Wipes]]
- [[Lore Market]]

Key decisions:

- The game launches alongside an official Lore, acquired in the [[Lore Market]].
- Without an [[Official Server]], seasons and wipes become configuration of each community server and each Lore.
- The server runs in Seasons.
- Each season ends in a narrative Cataclysm.
- The Hard Wipe erases cities, inventories, gold, markets, properties and territorial control.
- Geography may change after each wipe.
- Character name, basic identity, Grimoire, unlocked abilities, titles and cosmetic relics are preserved.
- The wipe prevents permanent monopolies without erasing account memory.

## 07 - Visual and Technical Direction

- [[Visual and Mechanical Direction]]
- [[Beta Asset Inventory]]

Key decisions:

- **Stylized painterly 3D**, restrained dark fantasy. Not 2D, not photorealism.
- Tactical camera, elevated and tilted, with limited rotation.
- **Terrain verticality is a game rule**, affecting stamina, routes, ambushes, gathering and city founding.
- Combat is precision action PvP, not a pure soulslike.
- **PixiJS is no longer a dependency of the final client.** The 3D engine choice (Godot, Unity or web 3D) will be validated in a separate prototype.
- The first prototype must prove a small enclosed region, not a complete open world.

## 08 - Descents, Cultures and Pantheons

The city's identity is assembled in three layers: **Descent** (permanent, chosen in the Stone Age), **Culture** (defined by the deity followed, switchable between Eras) and **Deity** (chosen every Era).

- [[Culture System]]
- [[Descent — Westerners]] · [[Descent — Easterners]] · [[Descent — Africans]] · [[Descent — Americans]]
- [[Era Progression]]
- [[Clan System]]
- [[Deities and Passives]]
- [[Divine Ult Rules]]
- 9 `Culture — <Name>` notes and 9 `Pantheon — <Name>` notes

Key decisions:

- **Four Descents**: Westerners (Norse, Greeks), Easterners (Mesopotamia, Sān Jiào), Africans (Egyptians, Yoruba), Americans (Aztecs, Maya, Tupi-Guarani).
- Four eras: Stone, Copper, Bronze and Iron. Limits of 20, 50, 100 and 150 citizens.
- **The Stone Age has no religion at all** and is identical for all cultures of the same Descent.
- Cultural traits only take effect in Copper, with the choice of the first deity — which **defines the city's culture**.
- Clans exist from the Stone Age and become formal institutions in Bronze, with seats and their own missions.
- **81 deities**: nine per culture, three per unlockable era.
- **Deities are era-locked.** A god exists only in its own era — every era transition forces a change of deity.
- Switching deity within the same culture carries no penalty. Switching to another culture of the same Descent triggers the **Wrath of the Abandoned God** for 24 hours. Switching Descent is impossible.
- **The Wrath is the exact inverse of the passive, at double the magnitude.** Copper gods punish production; Bronze, structure and relations; Iron, assets accumulated across the entire run.
- Each deity grants a permanent city passive (~5% in Copper, ~10% in Bronze, ~15% in Iron).
- Each deity offers three Ultimate paths — Attack, Defense and Mobility — totaling **243 ults**.
- Ult AoE scales by era: Copper single target, Bronze up to 3×3, Iron up to 5×5.
- This pillar closes three GDD gaps: Technological Eras, Sacred Temple and Divine Ultimate.

## 09 - Editor Mode, Mods and Distribution

The game is an open platform. The core loop is one product; content authoring is another.

- [[Editor Mode]]
- [[Mods and Extensibility]]
- [[Lore Market]]
- [[Official Server]]

Key decisions:

- The playable client is free and Open Source.
- Playing community Lores never costs anything through the base game.
- Creating content requires unlocking Editor Mode: R$ 10.00, one-time payment, per account.
- Mods are open, with no fee and no prior approval.
- The Editor ships with content pipeline mods, including 3D model import.
- Official Lores are sold in the Lore Market.
- A community Lore sold in the Market pays 10% to the game; distributed outside the Market, it pays 0%.
- Community Lores may be free or follow the creator's own rules.
- There is no other monetization of the game itself.
- The Official Server is out of scope.

---

## Current Project State

The conceptual GDD is structured across the game's main pillars. Visual direction is approved and the technical architecture needs revision after the shift to 3D. **The monorepo does not exist yet.**

## Next Steps

1. Validate the 3D engine choice in a separate prototype.
2. Revise the technical architecture after that decision.
3. Create the `aetherna/` monorepo.
4. Configure `apps/web-client` and `apps/game-server`.
5. Create `packages/shared-*`.
6. Define the first Drizzle/PostgreSQL models: Account, Character, Session, WorldPosition, Inventory, Item, City, Property, MarketListing, Season.

## Project Risks

| Risk | Nature |
|---|---|
| Excessive economic complexity before a playable MVP | Scope |
| Political scope larger than the initial infrastructure supports | Scope |
| Combat and movement demanding low latency before the base is stable | Technical |
| Contract divergence between client and server | Technical |
| **3D shift invalidating part of the approved architecture** | Technical |
| Open Source model with a payment gate on Editor Mode: how the unlock holds up in an open-source client | Business |
| Revenue concentrated in two narrow sources, with no recurring subscription income | Business |
| Lore Market requiring curation, moderation, refunds and creator payouts | Product |
| Open mods executing third-party code, requiring a sandbox | Security |
| Without an Official Server, adoption depends on the community hosting servers with low friction | Adoption |
| **Culture scale conflict**: source documents describe cities of 20–150 citizens run by "the player"; the vault describes cities governed by many players | Design |
| Volume of content: 81 deities and 243 ults need balancing, art and implementation | Production |
| Grid-based tactical ult rules versus precision action PvP combat — still unreconciled | Design |
| Dependence on critical mass: without a coordinated initial population there is no Town Hall, therefore no Citizenship | Adoption |
| Mandatory open-world VoIP as an accessibility barrier and unbudgeted infrastructure cost | Technical |

## Management Directive

Aetherna must be developed in layers.

First, prove the minimum technical loop: enter the world, see other players, move, gather, persist and die.

Then expand into local economy, caravans, urban politics, religion, wars and wipes.

Every new system must be born documented, typed, testable and connected to the GDD.
