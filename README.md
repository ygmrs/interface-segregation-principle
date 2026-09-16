# Interface Segregation Principle

A focused Java example of the Interface Segregation Principle (ISP), demonstrating how smaller, client-specific interfaces reduce unnecessary dependencies and improve object-oriented design.

## Overview

The Interface Segregation Principle is the **I** in SOLID:

> Clients should not be forced to depend on methods they do not use.

Instead of designing large general-purpose interfaces, ISP encourages interfaces that expose only the behavior required by their clients.

This reduces coupling and keeps implementations focused on the capabilities they actually support.

## Design Concept

Without interface segregation, a class may be forced to implement operations that are irrelevant to its responsibility.

```text
Large Interface
    │
    ├── Operation A
    ├── Operation B
    └── Operation C
           │
           ▼
    Client must depend
    on all operations
```

Applying ISP separates those responsibilities:

```text
Client A ──▶ Interface A ──▶ Implementation A

Client B ──▶ Interface B ──▶ Implementation B
```

Each client depends only on the contract it requires.

## Technical Focus

- Java
- SOLID principles
- Interface Segregation Principle
- Object-oriented programming
- Interface design
- Loose coupling
- Maintainable software design

## Repository Structure

```text
interface-segregation-principle/
├── src/
├── .gitignore
└── README.md
```

The Java implementation is located under `src/`.

## Why Interface Segregation Matters

Applying ISP helps:

- avoid large, overly broad interfaces
- reduce unnecessary dependencies
- prevent implementations from supporting irrelevant operations
- keep contracts cohesive and easier to understand
- make software easier to extend and maintain

## Purpose

This repository provides a compact implementation example of one of the core SOLID design principles and serves as a reference for client-focused interface design.
