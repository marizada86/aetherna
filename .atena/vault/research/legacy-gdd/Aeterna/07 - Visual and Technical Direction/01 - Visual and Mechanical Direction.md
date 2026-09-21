---
tags:
  - gdd
  - visual-direction
  - 3d
  - combat
  - beta
categoria: "[[07 - Visual and Technical Direction]]"
status: approved
---

# Visual and Mechanical Direction

## Product Decision

Aetherna will be a sandbox MMO in **stylized painterly 3D**, with restrained dark fantasy. It will not use 2D art as its final direction, nor pursue photorealism.

The primary visual reference is **No Rest for the Wicked**, used only as a reference for language: depth, materials with a painted finish, environment scale, elevated camera and atmosphere. Aetherna does not copy assets, narrative, characters, world or systems from that game.

## Visual Goals

- Communicate that the world is beautiful, hostile and physically material.
- Keep characters, weapons, cargo, buildings, hazards and abilities legible at medium camera distance.
- Use geography, architecture and lighting to convey risk and opportunity without relying on the interface alone.
- Enable modular production and consistent performance in multiplayer scenes.

## Artistic Language

- 3D models of moderate complexity, with strong silhouettes.
- Stylized textures and materials, with wear, brush strokes and controlled color variation.
- Environmental scale larger than that of characters, to convey vulnerability and the grandeur of the world.
- Directional lighting, fog and point lights such as torches, windows, braziers and campfires; atmospheric effects may never hide combat information.
- Contextual color palette: nature and settlements use earthy tones; war, crime, corruption and cataclysms receive their own chromatic languages.
- Cosmetics preserve the readability of weapon, stance, faction and cargo volume.

## Camera and Navigation

The camera is tactical, elevated and tilted, with moderate perspective. It is not a flat isometric board.

- Close zoom for combat, gathering and interiors; medium zoom for exploration; wide zoom only in safe or strategic situations.
- Rotation limited to fixed increments to preserve orientation and competitive fairness.
- Roofs, canopies and walls that obstruct the character become translucent or temporarily hidden.
- The camera may not reveal enemies, routes or areas outside the expected field of play.
- Special scenes, such as walls, bridges, mines and temples, may use contextual framing without removing player control.

## Verticality as a System

Terrain height is a game rule, not just decoration. Cliffs, slopes, stairs, walls, bridges, rivers, ravines, caves and narrow passages affect:

- stamina cost and movement speed;
- routes and safety of [[Caravan Logistics|caravans]];
- ambushes, defense and lines of sight in PvP;
- economic value and risk of gathering;
- founding, expansion and defense of cities;
- the effects of cataclysms on geography.

## Combat: Precision Action PvP

Combat will not be a pure soulslike. It will be **precision action PvP**: positioning, range, execution timing, stamina and reading intent all matter, but the implementation is designed for latency and multiplayer groups.

- Each weapon and ability has clear range, wind-up, execution and recovery.
- Dodges and blocks consume resources and demand decisions; there is no unlimited mobility.
- Dangerous attacks, crowd control and ultimates have consistent visual telegraphing and predictable hitboxes.
- The system preserves the loadout of 3 profession abilities and 1 ultimate described in [[3-Ability Combat System]].
- Extreme-precision parry is not a central requirement of competitive PvP.
- Visual effects prioritize information and never obscure targets, impact areas or scenery resources.

## Technical Consequence

The approved direction requires a client with 3D rendering, perspective camera, vertical terrain, character animation and real-time lighting. Therefore, **PixiJS is no longer a dependency of the final client**.

The choice of 3D engine will be validated in a separate prototype before rewriting the architecture. The decision must compare Godot, Unity and web 3D solutions against the requirements of multiplayer performance, asset pipeline, export and maintenance.

## Scope of the First Prototype

The first prototype must prove a small, enclosed region, not a complete open world:

1. camera, zoom, occlusion and limited rotation;
2. multiplayer movement with terrain height;
3. a route with a road, a steep shortcut, a bridge and a chokepoint;
4. gathering of wood, stone and ore;
5. combat against one enemy and optional PvP duel;
6. stamina, cargo and basic death/respawn;
7. authoritative synchronization of position, action and essential state.

The production inventory for the beta is in [[02 - Beta Asset Inventory]].
