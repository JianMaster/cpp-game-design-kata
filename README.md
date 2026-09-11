# C++ Game Design Kata

A focused training repository for improving the ability to turn game-system requirements into implementable C++ designs.

The goal is not to collect design patterns or build large demo games. Each kata trains the same conversion chain:

**Requirement → Execution Flow → State Changes → Responsibilities → Interfaces → Implementation → Refactoring → Retrospective**

## Training rules

1. One small game-system problem per week.
2. Before coding, complete the week's `design.md`.
3. Keep the first design small. Do not add abstractions only for hypothetical future requirements.
4. Prefer 3–5 core domain types unless the problem clearly requires more.
5. Do not use `Manager`, `System`, `Service`, `Controller`, or `Factory` as a substitute for an unclear responsibility. If you use one, explain its concrete job.
6. Implement the smallest version that satisfies the acceptance criteria.
7. After implementation, compare the final code with the original design and complete `retrospective.md`.
8. AI may review your reasoning, point out missing cases, and challenge design choices. Do not ask AI for the complete solution before producing your own design.

## C++ focus

Besides system design, each week will emphasize one or two C++ engineering topics that matter in game-programming interviews and production code: value/reference/pointer semantics, `const`, RAII, ownership, STL containers, polymorphism vs composition, move semantics, lifetime management, testing, allocations, and basic performance reasoning.

## Weekly structure

```text
weeks/
  01-damage-resolution/
    requirements.md
    design.md
    retrospective.md
```

Your implementation can add `include/`, `src/`, `tests/`, and `CMakeLists.txt` inside each week's directory as needed.

## What counts as progress

Finishing code is not enough. Weekly review focuses on:

- how quickly a requirement becomes an executable design;
- whether the execution path is complete;
- whether state changes and failure paths are identified;
- whether responsibilities and data ownership are clear;
- whether interfaces are sufficient without over-design;
- how much the final implementation differs from the initial design;
- whether rework decreases over time;
- whether C++ semantics are chosen intentionally and can be explained.

The long-term target is to receive an unfamiliar game-system requirement and reach a small, defensible, implementable design without getting stuck between architecture and code.
