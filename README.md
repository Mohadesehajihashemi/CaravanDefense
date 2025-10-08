# CaravanDefense (Scratch)

**Scratch Project URL:** https://scratch.mit.edu/projects/YOUR_PROJECT_ID/  
**Download:** [CaravanDefense.sb3](CaravanDefense.sb3)

## How to Play
- **Start:** Click the green flag.
- **Controls:** Arrow keys (↑ ↓ ← →) steer the caravan (llama). The caravan bounces off the stage edges.
- **Objective:** Collect diamonds (+5 Resources) and avoid the thief (−5 Resources).
- **Win/Lose:** Win at Resources ≥ 50 (“You Win”). Lose at Resources < 1 (“Game Over”).

## Implementation Highlights
- **Variable:** `Resources` (initialized to 20).
- **Custom Block:** `collectResources(amount)` → increments `Resources`, plays pickup sound, and checks win (`Resources > 49`) → broadcasts `You Win`.
- **Enemy AI:** Thief points toward `Caravan` and moves in a `forever` loop; on collision subtracts 5 with a short cooldown.
- **Broadcasts:** `Collected` (pickup), `Game Over` (loss), `You Win` (victory).
- **Player Control:** Four `key ... pressed?` checks set direction; continuous movement + `if on edge, bounce`.
- **(Optional) Stage Backdrops:** `Play`, `YouWin`, `GameOver` switched on start and on broadcasts.

## Assets
- Sprites: Caravan (llama), Characters 1 (thief), ResourceItem (Diamond).
- Graphics and sounds from the Scratch library (e.g., “snort” for pickup).

*Created by Mohadeseh.*
