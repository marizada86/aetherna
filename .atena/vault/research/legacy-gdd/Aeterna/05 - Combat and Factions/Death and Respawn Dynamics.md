# Death and Respawn Dynamics
**Category:** [[05 - Combat and Factions]]

## The Physical Checkpoint
On death, the player does not spawn at Ground Zero, but in the bed of their own house (recorded as a checkpoint).
* **The Destruction Factor (Homeless):** If the player's house is destroyed during an invasion but they still hold Citizen status in that city, the server respawns them in the nearby surroundings (borders) of the city, forcing a walk back to the conflict.

## Death Timer Escalation
To prevent the zombie tactic (dying and returning repeatedly to the front line), respawn time is cumulative.
* **Initial Death:** 30 seconds of grey screen.
* **Accumulation:** Each consecutive death adds +30 seconds to the timer.
* **Maximum Ceiling:** The dead-time limit is 5 minutes.

## Cooldown (System Forgiveness)
The death count cools down through active survival. For every 5 minutes the player spends alive in the world, the server reduces their next death timer by 30 seconds, until it returns to the minimum floor (30 seconds).
