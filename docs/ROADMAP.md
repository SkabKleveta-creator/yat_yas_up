# YAT YAS UP — Roadmap

## Current state

Current active prototype direction: **v0.3.5**  
Current lane: **planning/control board with guided playthrough**

The project is no longer being treated as a conventional mini-game. It is now a tabletop-style planning, control, trial, recovery, and AAR engine.

## Roadmap principle

Do not expand combat complexity before the player understands the board.

The order is:

1. clarity,
2. phase guidance,
3. selection/action usability,
4. pressure/screening clarity,
5. recovery route clarity,
6. AAR learning loop,
7. only then deeper planning economy.

## v0.3.x — Guidance and usability track

Purpose:

Make the current logic understandable to a first-time player.

Focus:

- Mission Coach improvements
- selection guidance
- action recommendations
- support marker clarity
- R7 route clarity
- roster accessibility
- right-side planning/control panel refinement
- AAR readability

Success condition:

A first-time player can complete a guided run without external explanation.

## v0.4 — Recovery and parts economy

Purpose:

Make recovery the mechanical heart of the game without becoming a repair simulator.

Potential features:

- recovery queue with visible queue entries
- one active R7 repair at a time
- parts readiness pool
- repair-forward / tow-to-R7 / leave-behind as abstract options
- R7 route timing
- degraded vehicle states based on abstract pips/stress
- AAR records recovery cost and missed recovery windows

Guardrail:

No real maintenance procedures, diagnosis, components, or vulnerabilities.

## v0.5 — Planning economy and trial setup

Purpose:

Make planning itself playable.

Potential features:

- Planning Points
- plan drawer
- route choice
- control-point placement cost
- R7 staging choice
- support marker pre-placement
- contingency cards as abstract game triggers
- plan-vs-actual AAR comparison

Guardrail:

Do not model real mission-planning products or procedures.

## v0.6 — AAR/debrief engine

Purpose:

Make the AAR the reason to replay.

Potential features:

- weighted category scoring
- Sustain / Fix / Next Trial Adjustment
- plan-vs-actual timeline
- top friction driver
- recovery cost summary
- command continuity summary
- pressure/screening effectiveness
- player notes export

Success condition:

The AAR produces one concrete next-trial adjustment that the player understands.

## Later optional layer — readiness campaign

Purpose:

Connect multiple trials into a lightweight readiness arc.

Potential features:

- persistent vehicle wear
- abstract readiness cards
- limited parts across multiple trials
- repeated beach/trial variations
- saved AAR history
- scenario seeds

Guardrail:

Keep this abstract. No real logistics procedures or technical maintenance modeling.

## Deferred or rejected for now

Do not prioritize:

- detailed enemy units,
- detailed weapon modeling,
- squad-level tactics,
- realistic fire support,
- realistic breach/obstacle procedures,
- casualty tracking,
- complex AI adversary behavior,
- full campaign before the single-board loop works.

## Current next recommended move

The next build should continue improving guided playthrough:

- clearer “what to do next” prompts,
- better action availability feedback,
- easier roster scanning,
- cleaner pressure/support marker explanations,
- stronger AAR recommendations.

Build depth only after first-time use is stable.
