---
tags:
  - gdd
  - assets
  - 3d-art
  - beta
categoria: "[[07 - Visual and Technical Direction]]"
status: planning
---

# Beta Asset Inventory

## Assumed Scope

This inventory covers a **foundational beta** of Aetherna: a persistent playable region with a starting city, wild periphery, mine, forest, road, bridge, bandit camp and a ruined point of interest. It supports the loops of nomad, citizenship, gathering, early crafting, combat, death/respawn, caravan and local market.

It does not include every biome, weapon, city, season, mount or content of the final version. Each asset below is required for the beta or for its production pipeline.

## Production Rules

- Create modular, reusable kits; do not model buildings, trees or rocks as unique pieces when a kit solves the case.
- Every asset must have documented naming convention, pivot, scale, collision, LODs and materials.
- Every character, enemy and interactive object needs a legible silhouette at medium camera distance.
- Variants by material, decal and color must produce diversity without multiplying unique models.
- Gameplay assets take priority over decoration.

## 1. Technical Foundations and Shared Art

| Group | Required assets | Initial quantity |
|---|---|---:|
| Base materials | wood, stone, earth, grass, sand, ferrous metal, noble metal, cloth, leather, water, glass and emissive | 12 families |
| Stylized PBR library | albedo, normal, roughness/metallic mask, color variation and wear for each family | 12 sets |
| Decals | mud, wagon track, crack, moss, blood, ash, burn, leaves and footprints | 9 types |
| Base VFX | dust, embers, smoke, fog, rain, splash, sparks, physical impact and magical glow | 9 systems |
| Base audio | footsteps per surface, impacts, wind, water, fire, wildlife, forest and city | 8 families |
| Icons and typography | grid, rarity frame, cursors, licensed fonts and status icons | 1 UI system |

## 2. Playable Characters

| Group | Required assets | Initial quantity |
|---|---|---:|
| Base body | male, female and neutral humanoid body, with skin tone variation | 3 base meshes |
| Heads and hair | compatible heads, haircuts, beards and eyebrows | 12 heads, 16 hairstyles, 8 beards |
| Skeleton and rig | one shared humanoid rig, hand/foot IK and equipment sockets | 1 master rig |
| Locomotion animation | idle, walk, run, turn, ascend, descend, swim, fall, land and carry weight | 10 sets |
| Action animation | gathering, mining, chopping, interaction, opening chest, eating, crafting, taking damage, death and respawn | 9 sets |
| Starting equipment | nomad clothing, citizen clothing, worker clothing, light leather and medium armor | 5 sets |
| Accessories | cloaks, backpacks, pouches, belts and lanterns | 12 pieces |

## 3. Weapons, Tools and Combat

| Group | Required assets | Initial quantity |
|---|---|---:|
| Weapons | short sword, battle axe, hammer, spear, bow and staff | 6 weapons |
| Tools | woodcutter's axe, pickaxe, sickle, artisan's hammer and gathering knife | 5 tools |
| Shields | wooden shield and metal shield | 2 models |
| Per-weapon animations | light attack, charged attack, block, dodge, impact, ability and death | 7 per category |
| Beta abilities | strike, bleed, stun, throw/thrust, shot, defensive zone and simple heal/support | 7 VFX + 7 icons |
| Combat feedback | area telegraphs, target marker, hit flash, optional numbers, poise bar and states | 6 systems |
| Consumable items | basic food, bandage, simple potion and repair kit | 4 models + icons |

## 4. Enemies, Wildlife and NPCs

| Group | Required assets | Initial quantity |
|---|---|---:|
| Passive wildlife | deer, boar and rabbit/small animal | 3 species |
| PvE enemies | wolf, melee raider, archer raider, city guard and corrupted creature | 5 archetypes |
| Enemy variations | color, equipment, size and accessories over the archetypes | 2 per archetype |
| Regional bosses | bandit leader and ruin creature | 2 unique enemies |
| City NPCs | mayor/councilor, merchant, blacksmith, guard, emissary and citizen | 6 archetypes |
| Animation and visual AI | locomotion, alert, attack, damage, death, patrol, conversation and work | 8 reusable sets per archetype |

## 5. Terrain, Biome and Navigation

| Group | Required assets | Initial quantity |
|---|---|---:|
| Modular terrain | flat ground, slope, step, cliff, riverbank, cave and mine entrance | 7 kits |
| Playable surfaces | earth, grass, stone, mud, wood, sand and shallow water | 7 navigation materials |
| Forest | 4 large trees, 3 young trees, 4 bushes, 5 rocks, fallen log, stump and exposed root | 19 prefabs |
| Mine and quarry | ore vein, gatherable stone, prop, beam, cart, rail, lantern and rubble | 8 prefabs |
| Ruins | wall, column, arch, stairway, floor, altar, statue, gate and debris | 9 modules |
| Water and crossing | river, bank, small bridge, wooden bridge, ford and decorative raft | 6 assets/systems |
| Roads and risk | dirt road, stone road, narrow trail, barricade, signage and abandoned outpost | 6 kits |
| Collision/navigation | colliders, navigation meshes, fall volumes, water volumes and climbing points | for each playable prefab |

## 6. Starting City and Properties

| Group | Required assets | Initial quantity |
|---|---|---:|
| Structural urban kit | foundation, wall, corner, door, window, floor, roof, stairs, balcony and chimney | 10 modules |
| Functional buildings | town hall, market, smithy, warehouse, tavern, temple, small house, medium house and guard post | 9 facades/sets |
| Street furniture | stall, barrel, crate, sack, parked wagon, post, torch, bench, well and sign | 10 prefabs |
| Player property | bed, chest, crafting table, campfire, door, fence and minimal decoration | 7 models |
| Defense and politics | short wall, gate, tower, banner, law board and bounty board | 6 models |
| Market | empty stall, active stall, coin/pouch, scale, contract and seal | 6 models/icons |

## 7. Caravans, Cargo and Logistics

| Group | Required assets | Initial quantity |
|---|---|---:|
| Vehicles | light wagon, cargo wagon and destroyed wagon | 3 models |
| Draft animals | pack horse/mule with harness | 1 species + 2 variations |
| Visible cargo | wood, stone, ore, crates, sacks, barrels and tarp-covered goods | 7 modules |
| Caravan states | empty, light, medium, heavy, damaged and destroyed | 6 visual configurations |
| Route gameplay | loading point, unloading point, road marker and danger sign | 4 prefabs |
| Looting | loot sack, broken crate, scattered resource and temporary ownership marker | 4 models/VFX |

## 8. Gathering, Crafting and Economy

| Group | Required assets | Initial quantity |
|---|---|---:|
| Gathering nodes | tree, stone, iron, herb, fiber and wild food | 6 types |
| Node states | intact, partially gathered, depleted and regenerating | 4 states per type |
| Production stations | workbench, forge, anvil, sawmill, mill and kitchen | 6 models |
| Inventory resources | wood, stone, ore, coal, fiber, leather, meat, food and ingot | 9 icons + world models |
| Starting products | plank, bar, rope, tool, simple weapon, simple armor and rations | 7 families |
| Item quality | common, refined and masterpiece | 3 frames, 3 effects and 3 visual marks |

## 9. Interface, UX and Accessibility

| Group | Required assets | Initial quantity |
|---|---|---:|
| HUD | health, stamina, cargo, compass, local chat, party, combat state and alerts | 8 components |
| Inventory | grid, tooltip, drag/drop, comparison, rarity and weight | 6 components |
| Combat | hotbar, cooldown, resource, target, telegraph and death/respawn | 6 components |
| World | local map, city map, route marker, property plaque and market | 5 components |
| Social/political | city identity, banner, criminal reputation, bounty and letter/emissary | 5 components |
| Accessibility | UI scaling, high contrast, remapping, effect reduction, subtitles and colorblind modes | 6 features |

## 10. Atmosphere, Season and Presentation

| Group | Required assets | Initial quantity |
|---|---|---:|
| Environmental cycle | morning, afternoon, night, rain, fog and wind | 6 profiles |
| Ambient sound | forest, mine, river, city, ruin, storm and distant combat | 7 soundscapes |
| Music | exploration, city, danger, combat, victory and death | 6 tracks or adaptive layers |
| Beta cataclysm | one visual corruption/collapse event with sky, particles, decals, audio and scene alteration | 1 complete set |
| Brand and presentation | logo, title screen, loading screen, key art and minimal capture kit | 5 assets |

## 11. Production Prioritization

### P0 — Required for the playable prototype

- humanoid rig, placeholder character, one weapon, one tool and locomotion animations;
- camera, vertical terrain, road, bridge, forest, mine and collision;
- one enemy, one wood node and one ore node;
- HUD for health, stamina, cargo and hotbar;
- minimal VFX and audio for attack, impact, gathering and death.

### P1 — Required for the functional beta

- all groups of characters, weapons, gathering, starting city, caravan, NPCs and interface listed above;
- two bosses, six functional buildings and local market;
- visual states for cargo, damage and looting;
- day/night cycle, simple weather and soundscapes.

### P2 — Polish before opening the beta to more players

- additional variations of NPCs, armor, enemies, vegetation and decoration;
- second layer of VFX and audio;
- the beta's visual cataclysm;
- full accessibility, presentation screens and key art.

## Out of Scope for the Foundational Beta

- multiple complete cities;
- all biomes and seasons;
- mounts beyond caravan draft animals;
- free building with hundreds of pieces;
- dozens of weapons and extensive ability trees;
- long cinematics and full voice acting;
- premium cosmetics at scale.

## Definition of Done

An asset enters the beta only when it has: final model or implementation, collision and navigation where applicable, LODs by distance, approved material, required variations, UI icon/feedback, matching audio/VFX, testing in a multiplayer scene and registration in the asset catalog.
