# Mods and Extensibility
**Category:** [[09 - Editor Mode and Mods]]

## Directive

Mods are **open**. The community can create mods freely, with no prior approval, no fee and no exclusivity.

The game does not monetize mods. See [[Open Source Model and Monetization]].

## Game Mods

Extend or alter the client and server: rules, UI, rendering, integrations. Installable by any player, without [[Editor Mode]].

## Editor Mods

Extend Editor Mode itself. The goal is for the Editor to ship with content pipeline mods from day one:

* 3D model import.
* Sprite, tileset and atlas import.
* Audio import.
* Procedural map and settlement generators.
* Lore package exporters and validators.

## Compatibility

A Lore can declare mods as dependencies. The client resolves and flags missing dependencies before entering a match. A Lore sold in the [[Lore Market]] must declare its dependencies explicitly.

## Open Questions

* Stable API surface of the mod loader.
* Sandbox and permission model for mods (risk of executing third-party code).
* License policy for mods redistributing third-party assets.
