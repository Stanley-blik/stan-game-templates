# Strategy RPG Builder Template

## Overview
A template for creating strategy RPG games with base construction, army management, and narrative campaign systems.

## Core Requirements
1. Base building and resource management systems
2. Army composition and tactical unit deployment
3. Branching narrative campaigns with choice consequences
4. Research and technology progression trees

## Recommended Structure
```
Project Root/
├── Assets/
│   ├── Scripts/
│   │   ├── BaseManagement/
│   │   ├── Army/
│   │   ├── Campaign/
│   │   └── UI/
│   ├── Prefabs/
│   │   ├── Buildings/
│   │   ├── Units/
│   │   └── CampaignEvents/
│   ├── Scenes/
│   └── Art/
├── ProjectSettings/
└── Packages/
```

## Essential Systems

### Base Construction System
- Purpose: Enable players to design and expand their headquarters
- Components: Building grid, resource connectors, upgrade paths
- Implementation: Modular construction with adjacency bonuses

### Army Composition System
- Purpose: Allow tactical customization of military forces
- Components: Unit roster, equipment loadouts, formation management
- Implementation: Slot-based system with synergy calculations

## Assets Required

### Strategic Assets
- Type: 3D Models/Sprites
- Quantity: 50-100 buildings and unit types
- Specifications: Clear visual hierarchy for strategic information

## Best Practices
- Design intuitive base layout with clear resource flow
- Balance army customization with accessible tactical depth
- Create meaningful narrative choices with lasting consequences

## Common Pitfalls
- Overwhelming base management with micromanagement
- Inconsistent difficulty progression in campaign missions

## References
- Strategy Game Economy Design
- Narrative Choice Implementation