# Zombie Game Template

## Overview
A template for creating zombie-themed games with survival horror, undead hordes, and post-apocalyptic settings.

## Core Requirements
1. Zombie AI with varied behaviors and movement patterns
2. Survival mechanics with health, resources, and shelter
3. Weapon and equipment systems for zombie combat
4. Post-apocalyptic environments with exploration elements

## Recommended Structure
```
Project Root/
├── Assets/
│   ├── Scripts/
│   │   ├── Zombies/
│   │   ├── Survival/
│   │   ├── Combat/
│   │   └── UI/
│   ├── Prefabs/
│   │   ├── Zombies/
│   │   ├── Weapons/
│   │   └── Environments/
│   ├── Scenes/
│   └── Art/
├── ProjectSettings/
└── Packages/
```

## Essential Systems

### Zombie AI System
- Purpose: Create varied undead enemies with distinct behaviors
- Components: Behavior manager, pathfinding system, animation controller
- Implementation: Configurable AI with different zombie types and tactics

### Survival Mechanics
- Purpose: Implement core survival elements like health and resources
- Components: Health system, hunger/thirst meters, inventory management
- Implementation: Layered survival systems with escalating tension

## Assets Required

### Zombie Assets
- Type: 3D Models and Audio
- Quantity: 20-50 zombie variants with animations and sound effects
- Specifications: Distinct visual designs with gore and decay effects

## Best Practices
- Design varied zombie behaviors to maintain tension and unpredictability
- Create atmospheric environments that enhance horror elements
- Balance resource scarcity to maintain challenge without frustration

## Common Pitfalls
- Making zombie AI too predictable or repetitive
- Poor difficulty progression leading to either constant fear or boredom

## References
- Zombie Game Design Principles
- Survival Horror Mechanics