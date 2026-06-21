# YAT YAS UP

**YAT YAS UP** is a planning/preparation tabletop-style prototype about building an abstract amphibious landing problem, launching an AAV platoon package through friction, managing command/control and recovery, and using the after-action review to improve the next trial.

This project is intentionally **not** a real-world tactics trainer. It uses public planning themes and game-safe abstractions only.

## Current prototype state

**Current design version:** v0.3.5  
**Prototype lane:** Planning and control board / TTRPG trial engine  
**Core loop:**

```text
PLAN → EXECUTE → DISRUPT → RECOVER → LEARN
```

The current build direction emphasizes:

- a board-first planning/control layout,
- left-side force roster and action screen,
- right-side mission coach and planning guidance,
- center tactical board,
- abstract friction markers,
- C2 net tether logic,
- dismount/screening mechanics,
- recovery coordination through the R7 and parts track,
- AAR-driven iteration.

## Force package

The current abstracted force package is:

| Asset | Count | Game role |
|---|---:|---|
| P7 | 8 | AAV platoon tracks |
| C7 | 1 | Beach command/control support node |
| R7 | 1 | Recovery/repair support track |

P7 roles:

| Track | Role |
|---|---|
| P7-1 | AAV Platoon Commander / command authority |
| P7-2 | AAV Platoon Sergeant / recovery coordination |
| P7-3 | Troop Carrier 1 |
| P7-4 | Troop Carrier 2 |
| P7-5 | Troop Carrier 3 |
| P7-6 | Troop Carrier 4 |
| P7-7 | C7 chase / support element |
| P7-8 | R7 chase / parts track |

Each troop carrier represents one abstract infantry bundle:

- Rifle Squad A
- Rifle Squad B
- Machine-gun support element
- Mortar / indirect support element

These are represented as game abstractions. No real-world employment procedures are modeled.

## Design identity

YAT YAS UP is best understood as a **planning and control mission board**:

1. Set the terrain/friction problem.
2. Establish control points.
3. Launch the AAV platoon.
4. Establish Beach C2.
5. Arrive and organize.
6. Dismount/screen.
7. Rally.
8. Remount.
9. Advance.
10. Recover degraded vehicles.
11. Run the AAR and adjust the next trial.

## Guardrails

This project must remain game-safe:

- No real-world tactics trainer.
- No weapon employment procedures.
- No targeting methods.
- No vulnerability modeling.
- No breach methods.
- No field-manual procedures.
- No casualty simulation.
- No realistic repair steps.
- Fire Support and MG Base affect abstract pressure/friction markers only.
- Vehicle movement must remain logically tied to board state and control-point sequencing.

## Repository documents

Start with:

- [`docs/DESIGN_LOCK.md`](docs/DESIGN_LOCK.md)
- [`docs/V0_3_LOGIC_LOCK.md`](docs/V0_3_LOGIC_LOCK.md)
- [`docs/PLAYTEST_GUIDE.md`](docs/PLAYTEST_GUIDE.md)
- [`docs/ROADMAP.md`](docs/ROADMAP.md)
- [`docs/GUARDRAILS.md`](docs/GUARDRAILS.md)
- [`docs/CHANGELOG.md`](docs/CHANGELOG.md)

## Current development emphasis

The next useful development work should focus on:

- guided playthrough clarity,
- visible phase progression,
- roster/action usability,
- support marker clarity,
- recovery route readability,
- AAR usefulness,
- avoiding overcomplexity.

The game is on the right path when a first-time player can understand:

> Select a track or marker, issue a phase-valid order, watch the trial resolve through friction, then read what held and what broke.
