# Platformer Legends Template

## Overview
A template for creating platformer games with precise movement mechanics, level design challenges, and character progression systems.

## Core Requirements
1. Precise platforming mechanics with jumping, wall-jumping, and special movement abilities
2. Challenging level design with environmental hazards and obstacle courses
3. Character progression systems with ability unlocks and power-ups
4. Collectible systems with hidden items and completion tracking
5. Visual feedback for player actions and environmental interactions
6. Multiple difficulty tiers with optional challenge elements

## Recommended Structure
```
platformer-legends/
├── assets/
│   ├── characters/
│   ├── environments/
│   ├── collectibles/
│   └── ui/
├── src/
│   ├── core/
│   │   ├── level_manager.py
│   │   ├── progression.py
│   │   └── collectible_system.py
│   ├── entities/
│   │   ├── player.py
│   │   ├── enemy.py
│   │   └── platform.py
│   ├── systems/
│   │   ├── movement.py
│   │   ├── collision.py
│   │   └── physics.py
│   └── ui/
│       ├── hud.py
│       ├── pause_menu.py
│       └── level_select.py
├── data/
│   ├── levels.json
│   ├── characters.json
│   └── collectibles.json
└── README.md
```

## Essential Systems
1. **Movement System** - Handles precise platforming controls with acceleration, momentum, and special abilities
2. **Collision System** - Manages interactions between player, enemies, and environmental elements
3. **Level Management** - Coordinates level loading, checkpoints, and progression
4. **Collectible System** - Tracks hidden items, secrets, and completion percentages
5. **Progression System** - Manages ability unlocks, power-ups, and character enhancements
6. **Physics System** - Implements gravity, momentum, and environmental interactions

## Assets Required
1. Character sprites with animation frames for running, jumping, and special actions
2. Environmental art with platforms, hazards, and interactive elements
3. Collectible item visuals with distinctive designs and pickup effects
4. UI elements for HUD displays, menus, and level selection
5. Sound effects for jumps, landings, collectibles, and environmental feedback
6. Music tracks that complement level themes and gameplay intensity

## Best Practices
1. Design tight controls with responsive input and predictable physics
2. Create levels with clear visual hierarchy guiding player movement paths
3. Implement fair checkpoint systems to reduce frustration from difficult sections
4. Provide visual feedback for player actions and environmental interactions
5. Balance difficulty progression to maintain challenge without excessive punishment
6. Include accessibility options for players with different reflexes and abilities

## Common Pitfalls
1. Inconsistent or imprecise controls leading to player frustration
2. Poorly placed hazards creating cheap deaths or unfair challenges
3. Overly punishing failure penalties that discourage continued attempts
4. Inadequate visual feedback making it difficult to judge distances or actions
5. Repetitive level design lacking variety in mechanics or environmental themes
6. Neglecting accessibility for players with different physical abilities

## References
1. [Platformer Design Principles](https://www.gamedevelopment.net/platformer-design-principles)
2. [Movement Mechanics in 2D Games](https://www.gamasutra.com/movement-mechanics-2d-games)
3. [Level Design for Platformers](https://www.gamesindustry.biz/level-design-platformers)