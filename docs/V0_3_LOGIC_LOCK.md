# YAT YAS UP — v0.3 Logic Lock

## Purpose

This document captures the locked v0.3 logic direction for the current prototype.

v0.3 prioritizes the core spatial/mechanical friction loops before expanding into deeper planning economies.

## v0.3 design priority

Primary focus:

1. C2 Net Tether
2. Dismount / Screening
3. Phase-gated planning/control flow
4. Abstract pressure management
5. Simplified recovery/repair route clarity
6. Weighted AAR feedback

Deferred focus:

- full planning-point economy,
- full embarkation/load order,
- rehearsal system,
- full recovery triage economy,
- campaign readiness layer.

## Locked phase list

The playable phase flow is:

```text
PLAN
LAUNCH
ARRIVAL
BEACH C2
DISMOUNT / SCREEN
RALLY / ORGANIZE
REMOUNT
FORWARD ADVANCE
AAR
```

## Locked control points

| Control point | Purpose |
|---|---|
| Center Beach | Touchdown / form-up reference |
| Beach C2 Anchor | C7 + support P7 command/control node |
| Arrival | Operating platoon arrival/form-up point |
| Dismount | Troop carriers begin screening sequence |
| Rally / Organize | Troop bundles become rallied |
| Remount | Troop bundles reorganize for mounted movement |
| Forward Advance | Inland advance objective |
| Recovery Control | R7 support/repair anchor |

## C2 Net Tether model

The single source of truth for C2 net value is the distance between the Platoon Commander P7 and the C7 / Beach C2 anchor.

Do not add a second parallel comms display layer.

The C2 Net value drives order latency and board feedback.

### Tunable values

- Optimal tether radius: **6 cells** — TUNABLE
- Warning tether radius: **9 cells** — TUNABLE
- Critical tether radius: **12 cells** — TUNABLE
- Base order latency: **800 ms** — TUNABLE
- Warning order latency: **1400 ms** — TUNABLE
- Critical order latency: **2200 ms** — TUNABLE
- Broken tether latency: **3000 ms** — TUNABLE

## Dismount / Screening model

Dismounted troop bundles reduce nearby abstract pressure effects.

This is not a tactical method. It is a game-safe pressure-control mechanic.

### Locked rule

- A troop carrier can generate a screening marker after reaching the Dismount phase.
- Screening affects adjacent cells within **1 cell radius** — TUNABLE.
- A screening marker reduces pressure-marker effect by **50%** while active — TUNABLE.
- If two screening markers overlap the same pressure marker, pressure effect is capped at **75% reduction** — TUNABLE.
- Mounted movement through unscreened pressure receives a **+20 bog stress** penalty — TUNABLE.
- Mounted movement through screened pressure receives only **+5 bog stress** — TUNABLE.

## Pressure and support actions

- MG Base reduces selected pressure marker strength by **25 points** — TUNABLE.
- Fire Support reduces selected pressure marker strength by **35 points** — TUNABLE.
- MG Base cooldown: **6 seconds** — TUNABLE.
- Fire Support cooldown: **8 seconds** — TUNABLE.
- Pressure marker strength range: **0–100**.
- A pressure marker at **0** is considered suppressed/cleared for scoring purposes.

MG Base and Fire Support never move vehicles.

## Recovery model for v0.3

v0.3 keeps recovery simplified.

- PSG coordinates recovery and stays with the operating platoon.
- R7 and P7-8 perform recovery/repair movement.
- R7 supports one active recovery/repair at a time.
- Degraded vehicles enter a simple queue if R7 is already busy.
- Repair restores abstract capability/readiness only.

### Tunable values

- Repair time: **12 seconds** — TUNABLE.
- Parts readiness penalty per active repair: **10 points** — TUNABLE.
- Vehicle is considered degraded at **50 HP or lower** or bog stress over **70** — TUNABLE.
- Vehicle is considered recovered when repair timer reaches **0** and HP is restored to **80** — TUNABLE.

## AAR categories

v0.3 AAR categories:

- Beach C2 Anchor
- C2 Net Tether
- Arrival Order
- Screening Coverage
- Pressure Management
- Command Continuity
- Recovery Posture
- Forward Advance

Each category should produce:

- rating,
- short explanation,
- Sustain / Fix line,
- Next Trial Adjustment.

## Explicit do-not-model list

Do not model:

- real tactics,
- weapon employment,
- targeting methods,
- breach methods,
- field procedures,
- communications procedures,
- vulnerability exploitation,
- vehicle-specific technical damage,
- casualty simulation,
- actual repair steps,
- real-world fire support processes,
- squad battle drills,
- realistic route clearance.

All mechanics must resolve as abstract board effects: pressure, friction, delay, screening, queue, pips, readiness, or AAR scoring.
