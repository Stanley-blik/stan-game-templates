# AR Evolution Template

## Overview
A template for creating augmented reality games with evolutionary mechanics, real-world creature collection, and location-based progression.

## Core Requirements
1. AR creature capture and evolution systems
2. Real-world location integration with GPS mapping
3. Creature customization and breeding mechanics
4. Social features and shared experiences

## Recommended Structure
```
Project Root/
├── Assets/
│   ├── Scripts/
│   │   ├── AR/
│   │   ├── Creatures/
│   │   ├── Location/
│   │   └── UI/
│   ├── Prefabs/
│   │   ├── Creatures/
│   │   ├── Markers/
│   │   └── Interfaces/
│   ├── Scenes/
│   └── Art/
├── ProjectSettings/
└── Packages/
```

## Essential Systems

### AR Creature System
- Purpose: Place and interact with virtual creatures in real-world space
- Components: Creature placer, animation controller, interaction manager
- Implementation: Integration with ARKit/ARCore for platform-specific features

### Evolution Mechanics
- Purpose: Allow creatures to develop and change over time
- Components: Stat tracker, evolution triggers, transformation system
- Implementation: Data-driven approach with visual transformation feedback

## Assets Required

### AR Creature Assets
- Type: 3D Models with Animations
- Quantity: 50-100 creatures with multiple evolution stages
- Specifications: Optimized models for real-time rendering with smooth animations

## Best Practices
- Design AR interactions that work in varied lighting conditions
- Create clear visual feedback for creature evolution
- Implement social features that encourage group participation

## Common Pitfalls
- Poor AR tracking stability causing creature jitter
- Unbalanced evolution mechanics leading to overpowered creatures

## References
- Augmented Reality Development Guidelines
- Creature Design Principles