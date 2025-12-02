# Metroidvania Shooter Template

## Overview
A template for creating Metroidvania-style games with exploration, ability-gated progression, and shooting mechanics.

## Core Requirements
1. Interconnected world design with ability-gated areas and backtracking paths
2. Shooting mechanics with weapon variety, upgrades, and combat encounters
3. Ability acquisition system with movement and combat powers
4. Exploration incentives with hidden areas, secrets, and collectibles
5. Map systems with discovery tracking and navigation aids
6. Progressive difficulty with enemy scaling and challenge areas

## Recommended Structure
```
metroidvania-shooter/
├── assets/
│   ├── characters/
│   ├── weapons/
│   ├── environments/
│   └── ui/
├── src/
│   ├── core/
│   │   ├── world_manager.py
│   │   ├── ability_system.py
│   │   └── exploration.py
│   ├── entities/
│   │   ├── player.py
│   │   ├── enemy.py
│   │   └── ability.py
│   ├── systems/
│   │   ├── combat.py
│   │   ├── movement.py
│   │   └── map.py
│   └── ui/
│       ├── hud.py
│       ├── map_screen.py
│       └── ability_menu.py
├── data/
│   ├── abilities.json
│   ├── weapons.json
│   └── areas.json
└── README.md
```

## Essential Systems
1. **World Management System** - Handles interconnected maps, loading zones, and ability gates
2. **Ability System** - Manages power acquisition, upgrades, and usage restrictions
3. **Combat System** - Implements shooting mechanics, weapon variety, and enemy encounters
4. **Exploration System** - Tracks secrets, collectibles, and area completion
5. **Map System** - Provides navigation aids, discovery tracking, and area visualization
6. **Progression System** - Coordinates ability acquisition and area accessibility

## Assets Required
1. Character sprites or models with animation sets for movement and combat actions
2. Weapon visuals with firing effects, upgrades, and distinct designs
3. Environment art with interconnected areas, ability gates, and hidden passages
4. UI elements for maps, ability displays, and combat information
5. Sound effects for weapon fire, ability usage, and environmental audio
6. Music tracks that adapt to exploration, combat, and discovery moments

## Best Practices
1. Design interconnected worlds with clear visual cues for ability requirements
2. Create meaningful ability upgrades that open new traversal and combat options
3. Implement fair checkpoint systems to reduce frustration from difficult sections
4. Provide clear feedback for combat actions and their tactical consequences
5. Balance exploration incentives with guided progression to prevent aimless wandering
6. Ensure accessibility options for players with different skill levels and preferences

## Common Pitfalls
1. Creating confusing world layouts that obscure ability gate requirements
2. Poor ability design leading to repetitive gameplay or underpowered options
3. Inadequate map systems making navigation difficult or frustrating
4. Overly punishing combat encounters that discourage exploration
5. Insufficient exploration incentives leading to unengaging backtracking
6. Neglecting accessibility for players with different physical abilities

## References
1. [Metroidvania Design Principles](https://www.gamedevelopment.net/metroidvania-design)
2. [Ability-Gated Progression](https://www.gamasutra.com/ability-gated-progression)
3. [Exploration Mechanics](https://www.gamesindustry.biz/exploration-mechanics)