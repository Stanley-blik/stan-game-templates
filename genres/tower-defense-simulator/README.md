# Tower Defense Simulator Template

## Overview
A template for creating tower defense games with strategic base placement, enemy wave management, and upgrade systems.

## Core Requirements
1. Strategic tower placement mechanics with resource constraints
2. Enemy waves with varying movement patterns and resistances
3. Tower upgrade paths with branching specialization options
4. Resource collection and management systems
5. Map design tools with pathing algorithms
6. Visual feedback for targeting and damage indicators

## Recommended Structure
```
tower-defense-simulator/
├── assets/
│   ├── towers/
│   ├── enemies/
│   ├── projectiles/
│   └── ui/
├── src/
│   ├── core/
│   │   ├── game_manager.py
│   │   ├── wave_controller.py
│   │   └── resource_system.py
│   ├── entities/
│   │   ├── tower.py
│   │   ├── enemy.py
│   │   └── projectile.py
│   ├── systems/
│   │   ├── pathfinding.py
│   │   ├── targeting.py
│   │   └── collision.py
│   └── ui/
│       ├── hud.py
│       ├── tower_menu.py
│       └── level_select.py
├── data/
│   ├── levels.json
│   ├── towers.json
│   └── enemies.json
└── README.md
```

## Essential Systems
1. **Wave Management System** - Handles enemy spawning, timing, and difficulty progression
2. **Tower Placement System** - Validates positions, handles resource costs, and manages placement restrictions
3. **Targeting System** - Implements various targeting strategies (closest, strongest, weakest, first)
4. **Upgrade System** - Manages tower enhancement paths and specializations
5. **Resource System** - Tracks currency, resource generation, and spending
6. **Pathfinding System** - Calculates enemy routes and determines valid placement areas

## Assets Required
1. Tower sprites with animation frames for idle, attacking, and upgrading states
2. Enemy sprites with walk cycles and death animations
3. Projectile sprites with movement effects
4. UI elements for menus, buttons, and HUD displays
5. Sound effects for tower placement, firing, enemy deaths, and upgrades
6. Background art for different map themes

## Best Practices
1. Implement a flexible wave configuration system using data-driven design
2. Use spatial partitioning for efficient collision detection with many entities
3. Design towers with clear visual distinctions for different types and levels
4. Provide visual feedback for targeting range and placement validity
5. Balance difficulty progression to maintain engagement without frustration
6. Optimize rendering for scenarios with numerous simultaneous effects

## Common Pitfalls
1. Overcomplicating upgrade trees leading to analysis paralysis
2. Poor enemy pathfinding causing unrealistic movement behaviors
3. Inadequate visual feedback making gameplay decisions unclear
4. Unbalanced difficulty curves that spike too sharply
5. Performance issues with many towers firing simultaneously
6. Unclear UI preventing players from understanding game state

## References
1. [Tower Defense Design Patterns](https://gamedevelopment.tutsplus.com/articles/tower-defense-design-patterns--cms-22849)
2. [Pathfinding Algorithms in Games](https://www.redblobgames.com/pathfinding/a-star/introduction.html)
3. [Game Balance Concepts](https://gamebalanceconcepts.wordpress.com/)