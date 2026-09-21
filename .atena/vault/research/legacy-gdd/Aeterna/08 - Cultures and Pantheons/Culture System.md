---
tags:
  - cultures
  - descent
  - pantheon
  - eras
categoria: "[[08 - Cultures and Pantheons]]"
status: revised
---

# Culture System

**Category:** [[08 - Cultures and Pantheons]]

A city's identity in Aetherna is assembled in three layers, chosen at different moments and with different degrees of freedom.

```
Descent    → chosen in the Stone Age · PERMANENT
   Culture → defined by the deity followed · switchable between Eras, at a cost
      Deity → chosen every Era · mandatory from Copper onward
```

## Layer 1 — Descent

Four Descents. Each groups cultures that share the same prehistoric origin.

| Descent | Cultures | Stone Age note |
|---|---|---|
| Westerners | Norse · Greeks | [[Descent — Westerners]] |
| Easterners | Mesopotamia · Sān Jiào | [[Descent — Easterners]] |
| Africans | Egyptians · Yoruba | [[Descent — Africans]] |
| Americans | Aztecs · Maya · Tupi-Guarani | [[Descent — Americans]] |

**Descent is permanent.** Once chosen, the city can never migrate to another. It defines the entire Stone Age package and limits which cultures will be available for the rest of the run.

### How the Descent Is Chosen

```
5 houses built close together in a habitable zone
  → unlocks construction of the Gathering Point
    → players choose the Descent
      → the city acquires that Descent's prehistoric package
```

The **Gathering Point** is the first political structure in the game. There, the city's next steps are decided by **in-person voting** — the orality of the Stone Age. No writing, no board, no remote voting: whoever is not physically present does not vote.

See [[Era Progression]] for the full mechanic and [[The Town Hall and the Council]] for the institutional lineage born here.

## Layer 2 — Culture

The city's culture is **not chosen directly**. It is a consequence of which deity the city follows. Following Thor makes the city Norse; following Athena makes it Greek.

This means culture is **switchable**, provided the new culture belongs to the same Descent.

| Culture | Descent | Notes |
|---|---|---|
| Norse | Westerners | [[Culture — Norse]] · [[Pantheon — Norse]] |
| Greeks | Westerners | [[Culture — Greeks]] · [[Pantheon — Greeks]] |
| Mesopotamia | Easterners | [[Culture — Mesopotamia]] · [[Pantheon — Mesopotamia]] |
| Sān Jiào | Easterners | [[Culture — Sān Jiào]] · [[Pantheon — Sān Jiào]] |
| Egyptians | Africans | [[Culture — Egyptians]] · [[Pantheon — Egyptians]] |
| Yoruba | Africans | [[Culture — Yoruba]] · [[Pantheon — Yoruba]] |
| Aztecs | Americans | [[Culture — Aztecs]] · [[Pantheon — Aztecs]] |
| Maya | Americans | [[Culture — Maya]] · [[Pantheon — Maya]] |
| Tupi-Guarani | Americans | [[Culture — Tupi-Guarani]] · [[Pantheon — Tupi-Guarani]] |

**Cultural traits only take effect in the Copper Age.** In the Stone Age the city is only its Descent. Greek and Norse are indistinguishable until the first temple.

From Copper onward, each culture defines: urban stage, form of government, buildings, military units, signature combat formation, exclusive cultural system, city and clan missions, and its pantheon of nine deities.

### Government Is Culture-Specific

There is no single political model. The Norse þing, the Greek agora, the Egyptian nomarch, the Aztec council of the calpulli and the Maya ajaw are different structures with different rules.

**Switching culture brings down the government.** Offices of the previous culture are abolished, laws and treaties must be revalidated, and the new form of government is chosen from the destination culture's options. The switch is a political refounding, not a bonus adjustment.

**Writing is a political advantage.** Cultures with writing replace in-person voting with recorded voting, codify laws, detect tax evasion and administer territory at a distance. Oral cultures — Yoruba and Tupi-Guarani — remain bound to in-person voting, but in exchange they are immune to record destruction, produce no interceptable letters and pay no bureaucratic cost.

See [[The Town Hall and the Council]].

## Layer 3 — Deity

**81 deities**: 9 per culture, 3 per unlockable era. The Stone Age has none.

| Era | Available deities | Ult scale |
|---|---|---|
| Stone | **None — there is no religion** | — |
| Copper | 3 per culture | Single target, no AoE |
| Bronze | 3 per culture | AoE up to 3×3 |
| Iron | 3 per culture | AoE up to 5×5 |

### Deities Are Era-Locked

**A god exists only in its own era.** Freyr is accessible in Copper and only in Copper. On advancing to Bronze, Freyr becomes unavailable — not as patron, not as secondary cult, not in any form.

Direct consequence: **every era transition forces a change of deity.** The city does not choose whether to change patron; only whom to change to.

### Choice Moments

| Transition | What happens |
|---|---|
| Founding → Stone | Choose the **Descent**. No deity |
| Stone → Copper | Choose the **first deity** among the three of Copper. The culture is defined here |
| Copper → Bronze | **Mandatory** choice among the three of Bronze |
| Bronze → Iron | **Mandatory** choice among the three of Iron |

Within a single era the deity does not change. The choice exists only at the transition.

### Cost of Switching

| Situation | Allowed | Cost |
|---|---|---|
| New deity, **same culture** | Yes | **None.** It is natural progression |
| New deity, **another culture of the same Descent** | Yes | **Wrath of the Abandoned God** — 24 hours |
| New deity, **another Descent** | No | — |

Switching culture is blasphemy. The abandoned god grows enraged and punishes the city.

### Wrath of the Abandoned God

**The punishment is the exact inverse of the abandoned god's passive**, applied for **24 hours**.

If Freyr granted +5% food production and productive farms, his wrath makes fields lose fertility and animals stop breeding. If Tyr granted Order and strength to warriors while treaties were honored, his wrath annuls all of the city's treaties.

Severity scales with the abandoned god's era:

| Era of the abandoned god | Reach of the wrath |
|---|---|
| Copper | Hits production — the resource or profession it favored |
| Bronze | Hits structure and relations — buildings, formations, clan loyalty |
| Iron | Hits what the city accumulated across the entire run — research, prestige, records, population |

Individual wraths are listed in the `Pantheon — <Culture>` notes. Full rules in [[Deities and Passives]].

### What the Deity Grants

**Permanent city passive** while the cult is active — ~5% in Copper, ~10% in Bronze, ~15% in Iron, always accompanied by a thematic effect and, in later eras, by a condition or risk.

**Three Divine Ultimate paths** — Attack, Defense and Mobility. The citizen picks one for the fourth loadout slot described in [[3-Ability Combat System]]. System total: **243 ults**.

**The ult belongs to the city, not the player.** It is tied to the deity, which is tied to the city. The player only holds it while a citizen of that city under that deity — the ult **does not enter the [[Grimoire]]** and does not travel with the character. Losing citizenship, migrating city or becoming a nomad costs the ult. Since deities are era-locked, **no player keeps the same ult for more than one era**.

Design effect: the fourth slot stops being personal progression and becomes **political dependency**. The Council's choice of deity sets the combat ceiling for the entire population.

## Fit Within the GDD

This system closes three gaps recorded in the GDD:

**Technological Eras.** [[The Town Hall and the Council]] described the Council voting on Era advancement without defining the tree. [[Era Progression]] is that tree.

**Sacred Temple.** The main systemic sink in [[The Tax and Gold System]]. It is also the building that allows choosing the deity, from Copper onward. The offerings demanded by Iron Age deities are the concrete mechanism of that drain.

**Divine Ultimate.** [[3-Ability Combat System]] defines the loadout as 3 profession abilities + 1 Divine Ultimate, without saying where the ultimate comes from. It comes from the patron deity.

Full chain:

```
5 houses → Gathering Point → Descent (Stone Age, no religion)
  → Council votes Era advancement
    → Era unlocks a trio of deities per culture
      → Temple chooses the deity → defines the culture
        → permanent city passive
        → Divine Ultimate available (1 of 3 paths)
          → new Era → previous deity expires → mandatory choice
            → same culture: free · another culture: Wrath, 24h
```

## Cultures and the Open Source Model

Under [[Open Source Model and Monetization]], Descents, cultures and pantheons are content. The launch official Lore defines which ship with the game; [[Editor Mode]] lets the community create their own Descents, cultures, pantheons and ults, distributed through the [[Lore Market]].

## Open Questions

* **Scale conflict.** The source documents describe the city as run by "the player", with clans as institutions and a limit of 20 to 150 citizens. The vault's GDD describes cities founded and governed by **multiple players**, with [[The Council]] elected among them. Are clans player guilds or NPC factions? Does the population limit count players or NPCs?
* Which Descents and cultures ship in the launch official Lore.
* How Descent interacts with [[Languages and Letter Security|the Language Barrier]] — is language per Descent or per culture? If per culture, switching culture rewrites the city's language and invalidates old letters.
* If a city is conquered and absorbed under [[War and Expansion Policy]], does it inherit the victor's Descent? Descent is permanent, but the city ceases to exist — the question probably dissolves.
* Who decides the culture switch, if it brings down the very body that decided it.
* Whether oral cultures need additional compensation to balance the administrative advantage of writing.
