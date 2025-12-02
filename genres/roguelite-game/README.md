# Roguelite Game Template

## Overview
A template for creating roguelite games with permadeath mechanics, procedural generation, and progressive unlock systems.

## Core Requirements
1. Procedural level generation with consistent themes
2. Permadeath with meaningful progression systems
3. Combat mechanics with weapon and ability variety
4. Unlockable content and persistent upgrades

## Recommended Structure
```
Project Root/
├── Assets/
│   ├── Scripts/
│   │   ├── Generation/
│   │   ├── Combat/
│   │   ├── Progression/
│   │   └── UI/
│   ├── Prefabs/
│   │   ├── Rooms/
│   │   ├── Enemies/
│   │   └── Items/
│   ├── Scenes/
│   └── Art/
├── ProjectSettings/
└── Packages/
```

## Essential Systems

### Procedural Generation System
- Purpose: Create unique levels for each playthrough
- Components: Room generator, connector system, theme applier
- Implementation: Template-based generation with random variation

### Progression Persistence
- Purpose: Maintain player advancement between runs
- Components: Unlock tracker, currency system, meta-progression
- Implementation: Save system with run-independent achievements

## Assets Required

### Modular Assets
- Type: 2D Sprites/3D Models
- Quantity: 100-200 modular pieces for procedural generation
- Specifications: Seamless connection points for random assembly

## Best Practices
- Design tight feedback loops for combat and exploration
- Create meaningful choices in item and build selection
- Balance difficulty progression to maintain tension

## Common Pitfalls
- Making early deaths feel excessively punishing
- Repetitive generation reducing sense of discovery

## References
- Roguelike Game Design Patterns
- Procedural Content Generation Techniques