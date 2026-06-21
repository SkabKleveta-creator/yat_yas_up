# YAT YAS UP — Design Lock

## Project identity

**YAT YAS UP** is a planning/preparation tabletop-style prototype and trial engine.

The player does not simply “win a level.” The player builds an abstract beach problem, launches a force package through friction, reacts through planning/control actions, reads the AAR, and improves the next trial.

## Core loop

```text
PLAN → EXECUTE → DISRUPT → RECOVER → LEARN
```

## Product lane

YAT YAS UP is:

- a planning and control board,
- a TTRPG-adjacent mission rehearsal prototype,
- a trial engine,
- a systems game about command continuity, recovery, pressure management, and learning from breakdowns.

YAT YAS UP is not:

- an arcade shooter,
- a real-world tactics trainer,
- a doctrine simulator,
- a weapon employment simulator,
- a casualty simulation,
- a detailed repair or maintenance trainer.

## Current force package

| Asset | Count | Game role |
|---|---:|---|
| P7 | 8 | AAV platoon tracks |
| C7 | 1 | Beach C2 support node |
| R7 | 1 | Recovery/repair support track |

## P7 role lock

| Track | Role | Locked behavior |
|---|---|---|
| P7-1 | Platoon Commander | Command authority; must be protected; central to C2 net tether |
| P7-2 | Platoon Sergeant | Coordinates recovery while staying with the operating platoon |
| P7-3 | Troop Carrier 1 | Carries abstract infantry bundle |
| P7-4 | Troop Carrier 2 | Carries abstract infantry bundle |
| P7-5 | Troop Carrier 3 | Carries abstract infantry bundle |
| P7-6 | Troop Carrier 4 | Carries abstract infantry bundle |
| P7-7 | C7 chase/support | Remains with C7 at Beach C2 anchor |
| P7-8 | R7 chase/parts | Supports R7 recovery/repair route |

## Command/control lock

- The Platoon Commander P7 is the AAV platoon command authority.
- The C7 is not the Platoon Commander. It supports the command/control net.
- The C7 plus P7-7 establish or support the Beach C2 Anchor.
- The C2 Net is represented through one game-safe tether value, not real communications procedures.
- Orders may resolve through abstract delay/latency; no real-world signal procedures are modeled.

## Recovery lock

- The Platoon Sergeant coordinates recovery and remains with the operating platoon.
- The R7 and P7-8 parts track perform the physical recovery/repair route.
- The R7 handles one active recovery/repair cycle at a time.
- Degraded vehicles are represented as abstract capability loss, not realistic vehicle damage.
- Repairs are abstract timers and readiness restoration only.

## Infantry bundle lock

Each troop carrier represents one abstract infantry bundle:

- Rifle Squad A
- Rifle Squad B
- Machine-gun support element
- Mortar / indirect support element

Infantry is not individually micromanaged. The bundle state is what matters:

```text
Mounted → Dismounting → Screening → Rallied → Remounting
```

## Support action lock

- **MG Base** affects abstract pressure/friction markers only.
- **Fire Support** affects abstract pressure/friction markers only.
- Neither action moves vehicles.
- Neither action models real targeting, fires, effects, weapon employment, or procedures.

## Control point lock

Current control points:

- Center Beach
- Beach C2 Anchor
- Arrival
- Dismount
- Rally / Organize
- Remount
- Forward Advance
- Recovery Control

## UI identity lock

The current screen concept is split-screen planning/control:

- left: Force Roster / Action Screen,
- center: board-first tactical surface,
- right: Mission Coach / Planning Screen,
- no persistent bottom drawer stealing map height.

## Player clarity target

A first-time player should understand this without reading external instructions:

> Select a track or marker, issue a phase-valid order, watch the board resolve through abstract friction, then use the AAR to improve the next trial.
