# Idle Legends Template

## Overview
A template for creating idle/incremental games with legendary themes, automatic progression, and engaging upgrade systems.

## Core Requirements
1. Automatic resource generation and accumulation
2. Deep upgrade and progression systems
3. Legendary character and item collection
4. Meaningful long-term goals and milestones

## Recommended Structure
```
Project Root/
├── Assets/
│   ├── Scripts/
│   │   ├── Idle/
│   │   ├── Upgrades/
│   │   ├── Collection/
│   │   └── UI/
│   ├── Prefabs/
│   │   ├── Characters/
│   │   ├── Items/
│   │   └── Interfaces/
│   ├── Scenes/
│   └── Art/
├── ProjectSettings/
└── Packages/
```

## Essential Systems

### Idle Resource Generation
- Purpose: Automatically generate resources over time
- Components: Generator manager, tick system, accumulation tracker
- Implementation: Time-based progression with offline calculation

### Upgrade System
- Purpose: Provide meaningful progression through character/item enhancement
- Components: Upgrade tree, cost calculator, effect applier
- Implementation: Multiplicative scaling with diminishing returns

## Assets Required

### Collection Assets
- Type: 2D Sprites/Icons
- Quantity: 200-500 visual elements
- Specifications: Distinct visuals for characters and items with rarity indicators

## Best Practices
- Design clear progression paths with meaningful rewards
- Create engaging visual feedback for resource accumulation
- Implement balanced scaling to maintain long-term engagement

## Common Pitfalls
- Poorly balanced progression leading to excessive grind
- Unclear upgrade paths causing player confusion

## References
- Idle Game Design Principles
- Progression System Design