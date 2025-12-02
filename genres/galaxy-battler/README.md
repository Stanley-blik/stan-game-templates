# Galaxy Battler Template

## Overview
A template for creating space combat games with starship customization, tactical battles, and galactic exploration.

## Core Requirements
1. Starship customization with modular components, weapon systems, and aesthetic options
2. Tactical space battles with positioning, shield management, and environmental hazards
3. Galactic exploration with star systems, planets, and points of interest
4. Resource management with currency, materials, and upgrade costs
5. Combat variety with different ship classes, weapon types, and tactical scenarios
6. Progression systems with unlocks, reputation, and story advancement

## Recommended Structure
```
galaxy-battler/
├── assets/
│   ├── ships/
│   ├── weapons/
│   ├── environments/
│   └── ui/
├── src/
│   ├── core/
│   │   ├── combat_manager.py
│   │   ├── exploration.py
│   │   └── progression.py
│   ├── entities/
│   │   ├── ship.py
│   │   ├── weapon.py
│   │   └── system.py
│   ├── systems/
│   │   ├── customization.py
│   │   ├── navigation.py
│   │   └── economy.py
│   └── ui/
│       ├── shipyard.py
│       ├── galaxy_map.py
│       └── combat_hud.py
├── data/
│   ├── ships.json
│   ├── weapons.json
│   └── systems.json
└── README.md
```

## Essential Systems
1. **Combat Manager** - Handles space battles, shield systems, and tactical positioning
2. **Exploration System** - Manages star systems, navigation, and point of interest discovery
3. **Progression System** - Tracks unlocks, reputation, and story advancement
4. **Customization System** - Implements ship modification, weapon installation, and aesthetics
5. **Navigation System** - Coordinates hyperspace travel, system transitions, and route planning
6. **Economy System** - Manages resource collection, trading, and upgrade costs

## Assets Required
1. Ship models with modular components and damage state variations
2. Weapon effects with distinctive visuals and impact animations
3. Environment art for star systems, planets, and space stations
4. UI elements for ship customization, navigation, and combat displays
5. Sound design for engine effects, weapon fire, and space ambiance
6. Music tracks that evoke cosmic wonder and combat intensity

## Best Practices
1. Design intuitive ship customization with clear visual feedback for modifications
2. Create balanced combat encounters with tactical depth and strategic positioning
3. Implement varied exploration content with meaningful discoveries and rewards
4. Balance resource management to maintain progression without excessive grinding
5. Provide clear navigation aids without overwhelming players with complexity
6. Ensure performance optimization for large-scale space battles and environments

## Common Pitfalls
1. Overcomplicating ship customization leading to analysis paralysis or poor choices
2. Poor combat balance with either overwhelming or trivial enemy encounters
3. Repetitive exploration content lacking variety in discoveries or challenges
4. Inadequate tutorial systems leaving players confused about core mechanics
5. Neglecting performance optimization leading to frame rate issues in battles
6. Insufficient feedback making it difficult to understand combat actions or consequences

## References
1. [Space Combat Design](https://www.gamedevelopment.net/space-combat-design)
2. [Ship Customization Systems](https://www.gamasutra.com/ship-customization)
3. [Galactic Exploration Mechanics](https://www.gamesindustry.biz/galactic-exploration)