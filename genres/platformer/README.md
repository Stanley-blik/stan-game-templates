# Platformer Game Template

## Overview
A template for creating 2D/3D platformer games with precise character movement, level design tools, and combat systems.

## Core Requirements
1. Character movement and jumping mechanics
2. Level design with platforms and obstacles
3. Enemy AI and combat systems
4. Collectibles and progression mechanics

## Recommended Structure
```
Project Root/
├── Assets/
│   ├── Scripts/
│   │   ├── Character/
│   │   ├── Level/
│   │   ├── Enemies/
│   │   └── UI/
│   ├── Prefabs/
│   │   ├── Characters/
│   │   ├── Platforms/
│   │   └── Enemies/
│   ├── Scenes/
│   └── Art/
├── ProjectSettings/
└── Packages/
```

## Essential Systems

### Movement System
- Purpose: Precise character movement and physics
- Components: Character controller, input handler, ground detection
- Implementation: Custom movement system with raycasting for ground detection

### Level System
- Purpose: Organize platforms, obstacles, and collectibles
- Components: Tilemap system, level manager, checkpoint system
- Implementation: Grid-based level design with trigger zones

## Assets Required

### Character Sprites/Models
- Type: 2D Sprite/3D Model
- Quantity: 1-3 characters with animations
- Specifications: Multiple animation frames for movement states

## Best Practices
- Implement coyote time for forgiving jumps
- Use layered collision detection for precise platforming
- Design levels with increasing difficulty progression

## Common Pitfalls
- Inconsistent jump physics feeling floaty or sticky
- Poorly placed platforms causing player frustration

## References
- Unity 2D Platformer Tutorial
- Character Controller Best Practices