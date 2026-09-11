# Week 01 — Initial Design

Complete this file **before writing implementation code**.

Do not try to make it elegant. The purpose is to force the architecture-to-code transition into explicit steps.

## 1. Entry point

What starts one attack?

Write the concrete operation in one sentence.

> TODO

## 2. Execution flow

Write the complete happy-path sequence as numbered steps.

Example format only:

1. ...
2. ...
3. ...

> TODO

## 3. State changes

List every piece of game state that can change during an attack.

For each one, write:

- owner;
- old value conceptually;
- new value conceptually;
- who is allowed to change it.

> TODO

## 4. Failure / rejected paths

List every reason the operation can be rejected **before** state is changed.

> TODO

## 5. Responsibilities

List the core types you think are needed.

For each type, describe its responsibility using verbs, not vague nouns.

Bad:

- `BattleManager`: manages battle.

Better:

- `Character`: owns HP and enforces valid HP changes.

> TODO

## 6. Data ownership

For each relationship between your types, answer:

- who owns the object?
- does another object need a reference, pointer, value copy, or only a parameter during a call?
- why?

> TODO

## 7. Interface draft

Write only declarations/pseudocode-level signatures, not implementation bodies.

Include the minimum methods you currently believe are necessary.

> TODO

## 8. Unknowns

What are you still unsure about before coding?

Examples:

- where should validation live?
- should damage calculation mutate anything?
- should attack return a result object?

Do not hide uncertainty. Record it.

> TODO

## 9. Design prediction

Before coding, answer these three questions:

1. Which part of this design are you most confident will survive implementation unchanged?
2. Which part is most likely to change?
3. What would cause you to introduce another type?

> TODO

## 10. Time-to-start metric

Record approximately how long it took from reading `requirements.md` until you felt ready to write the first implementation line.

> TODO
