# YAT YAS UP — Repository Handoff

## Repository purpose

This repository holds the design documentation and prototype artifacts for **YAT YAS UP**, a planning/preparation TTRPG-style board and trial engine.

## Current design summary

YAT YAS UP is about managing an abstract force package through a planned beach landing sequence, command/control friction, pressure markers, dismount/screening, recovery/repair support, and AAR learning.

The player should feel like they are running a tabletop planning board, not piloting a shooter.

## Current active build concept

Latest discussed build: **v0.3.5**

Primary layout:

- left panel: Force Roster / Action Screen
- center: tactical planning board
- right panel: Mission Coach / Planning Screen

Primary logic:

- C2 Net Tether
- phase-gated orders
- dismount/screening pressure reduction
- MG and Fire Support pressure-only effects
- PSG coordinates recovery
- R7 and parts track perform recovery/repair route
- AAR produces learning feedback

## Immediate next development objective

Improve first-time usability.

A new player should not feel like they are clicking experimentally. The game should actively guide them through:

1. selecting a unit or marker,
2. issuing a valid order,
3. understanding the current phase,
4. seeing the effect on the board,
5. reaching the AAR,
6. understanding what to change next time.

## Suggested next patch name

**v0.3.6 — Guided Run Clarity Pass**

Potential patch items:

- make Mission Coach more directive,
- add “Next Recommended Click,”
- gray out invalid orders with reason text,
- add quick tooltip for selected track/marker,
- add “Why this matters” line for every phase,
- add clearer transition prompt when phase advances,
- make AAR recommendation more actionable.

## Hard stop rules

Stop and reassess if the build starts to feel like:

- an RTS,
- a shooter,
- a doctrine trainer,
- a realistic combat simulator,
- a maintenance trainer,
- a UI with too much hidden state.

## Preferred development rhythm

1. One focused patch.
2. Syntax/runtime smoke check.
3. Playtest by screenshot.
4. User feedback.
5. Update docs if logic changes.
6. Repeat.

## Document map

- `README.md` — public project overview
- `docs/DESIGN_LOCK.md` — design identity and locked project rules
- `docs/V0_3_LOGIC_LOCK.md` — v0.3 mechanics lock
- `docs/PLAYTEST_GUIDE.md` — how to test current prototype usability
- `docs/ROADMAP.md` — staged development path
- `docs/GUARDRAILS.md` — safety/abstraction boundaries
- `docs/CHANGELOG.md` — prototype history
