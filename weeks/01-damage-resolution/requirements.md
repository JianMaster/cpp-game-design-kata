# Week 01 — Damage Resolution

## Goal

Train the ability to turn a small game rule into a concrete, implementable design before writing code.

This is deliberately a small problem. Do not turn it into a full combat framework.

## Requirements

Implement a small RPG-style damage-resolution module.

A character has:

- current HP;
- maximum HP;
- attack power;
- defense power;
- alive/dead state derived from HP.

An attack has:

- an attacker;
- a target;
- a base damage multiplier;
- an optional critical hit flag.

Damage rules:

1. Raw damage = attacker attack power × base damage multiplier.
2. A critical hit multiplies raw damage by `1.5`.
3. Final damage = raw damage − target defense power.
4. Final damage can never be lower than `1`.
5. Damage is applied to the target HP.
6. HP cannot fall below `0`.
7. A dead target cannot be attacked.
8. An attacker that is dead cannot attack.

## Acceptance criteria

Your implementation must demonstrate at least these cases:

- normal attack;
- defense reducing incoming damage;
- minimum damage of 1;
- critical hit;
- target HP clamped to 0;
- dead attacker rejected;
- dead target rejected.

You may use assertions or a small test executable. Do not add a test framework unless you already know one and can set it up quickly.

## Constraints

- Use C++17 or later.
- Keep the domain design small: target roughly 2–5 core types.
- Do not add UI, engine code, rendering, ECS, serialization, networking, events, factories, dependency injection, or data-driven configuration.
- Do not introduce inheritance unless you can explain why it is required by the current requirements.
- Do not create a generic combat framework for hypothetical future features.

## C++ focus for this week

Be able to explain every use of:

- value vs reference;
- `const`;
- public getter vs mutating method;
- whether a pointer is needed anywhere;
- why your chosen types own or do not own other objects.

You are not graded on using advanced C++. Simple, intentional C++ is better than clever C++.

## Before writing implementation code

Complete `design.md` first and commit it separately.

Recommended commit sequence:

1. `week01: add initial design`
2. `week01: implement damage resolution`
3. `week01: refactor after implementation`
4. `week01: add retrospective`

This separation matters because the weekend review needs to compare your initial design with what you actually built.
