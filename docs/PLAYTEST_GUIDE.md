# YAT YAS UP — Playtest Guide

## Purpose

Use this guide to test whether YAT YAS UP is understandable as a planning/control board rather than an arcade game.

The goal is not to test player reflexes. The goal is to test whether the player understands:

1. what phase they are in,
2. what to select,
3. what actions are valid,
4. how pressure and screening work,
5. what the R7 is doing,
6. what the AAR is telling them to change.

## Current prototype behavior to test

Current version target: **v0.3.5**

Primary areas:

- Mission Coach clarity
- Force Roster / Action Screen usability
- center board readability
- C2 Net Tether feedback
- pressure marker readability
- MG / MTR support marker placement
- R7 recovery/repair route clarity
- AAR usefulness

## First-time player script

Ask the player to open the game without explaining the system in detail.

Give only this instruction:

> Try to run the board from Plan through AAR. Use the Mission Coach if you get stuck.

Observe whether they can:

- identify the roster,
- identify the map,
- identify the right-side guidance panel,
- select a track or group,
- issue an order,
- understand the current phase,
- tell what pressure markers are,
- explain what MG / MTR markers do,
- understand that Fire Support and MG Base affect pressure only,
- understand that PSG coordinates while R7 performs recovery,
- reach the AAR.

## Key playtest questions

### Usability

- Did the player know what to click first?
- Did the player understand that selection happens before action?
- Did the player use the Mission Coach?
- Did the player notice recommended actions or highlights?
- Did the player find the full roster without fighting the scroll?
- Did the right-side planning/control screen help or clutter?

### Board readability

- Could the player identify Water Lane, Surf, Beach/C2, and Inland zones?
- Could the player identify Center Beach, Beach C2 Anchor, Arrival, Dismount, Rally, Remount, Forward Advance, and Recovery Control?
- Could the player tell the difference between vehicles, support markers, and pressure markers?
- Did any marker look like a real tactical instruction rather than an abstract board symbol?

### Mechanics comprehension

- Did the player understand the C2 Net Tether?
- Did the player understand that C7 supports the net but does not command the platoon?
- Did the player understand that P7-1 commands the AAV platoon?
- Did the player understand that P7-2 coordinates recovery?
- Did the player understand that R7 and P7-8 perform the recovery/repair route?
- Did the player understand that dismount/screening reduces pressure effects abstractly?

### AAR usefulness

- Did the AAR explain what held?
- Did the AAR explain what broke?
- Did the AAR recommend a next-trial adjustment?
- Did the player want to run another trial?

## Pass / fail criteria

### Pass

A first-time player can explain the game in their own words as:

> I set up the board, move through phases, use the roster to issue orders, screen pressure, keep the net connected, recover degraded tracks with R7, and then read the AAR.

### Fail

The build needs another guidance/layout pass if the player says:

- “I do not know what I am supposed to do.”
- “I am just clicking to see what happens.”
- “The fire button moved a vehicle.”
- “I thought C7 was the commander.”
- “I thought PSG was towing the vehicle himself.”
- “I cannot tell what the adversary/pressure markers are.”
- “I cannot see the roster.”
- “The AAR is just a score, not a lesson.”

## Known watch items

- Avoid too many always-visible controls.
- Keep the center map dominant.
- Keep guidance active but not intrusive.
- Do not let support actions trigger vehicle movement.
- Keep recovery logic visually clear.
- Keep the project from drifting into doctrine or real tactics.

## Recommended next playtest focus

For the next session, test only three questions:

1. Can the player complete a guided run without external explanation?
2. Can the player correctly explain PSG/R7 recovery responsibility?
3. Does the AAR make the player want to change the next plan?
