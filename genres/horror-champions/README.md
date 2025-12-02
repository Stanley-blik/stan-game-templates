# Horror Champions Template

## Overview
A template for creating horror games with survival mechanics, psychological tension, and atmospheric storytelling.

## Core Requirements
1. Atmospheric horror elements with sound design, lighting, and environmental storytelling
2. Survival mechanics with resource scarcity, health management, and crafting systems
3. Psychological tension through pacing, jump scares, and narrative unease
4. Enemy AI with unpredictable behavior patterns and threat escalation
5. Player progression with skill development and equipment upgrades
6. Multiple endings based on player choices and performance

## Recommended Structure
```
horror-champions/
├── assets/
│   ├── characters/
│   ├── environments/
│   ├── sounds/
│   └── ui/
├── src/
│   ├── core/
│   │   ├── horror_system.py
│   │   ├── survival.py
│   │   └── progression.py
│   ├── entities/
│   │   ├── player.py
│   │   ├── enemy.py
│   │   └── item.py
│   ├── systems/
│   │   ├── ai.py
│   │   ├── atmosphere.py
│   │   └── crafting.py
│   └── ui/
│       ├── hud.py
│       ├── inventory.py
│       └── map.py
├── data/
│   ├── enemies.json
│   ├── items.json
│   └── story.json
└── README.md
```

## Essential Systems
1. **Horror System** - Manages atmospheric tension, jump scares, and psychological unease
2. **Survival System** - Handles health, resources, crafting, and environmental hazards
3. **AI System** - Implements enemy behavior, threat escalation, and unpredictability
4. **Atmosphere System** - Controls lighting, sound design, and environmental storytelling
5. **Progression System** - Manages skill development, equipment upgrades, and unlocks
6. **Narrative System** - Coordinates story branches, endings, and player choice consequences

## Assets Required
1. Character models with detailed animations for fear reactions and survival actions
2. Environment art with atmospheric lighting, shadows, and unsettling details
3. Sound design with ambient noises, musical tension, and jump scare audio cues
4. UI elements for survival stats, inventory management, and map navigation
5. Particle effects for atmospheric elements like fog, dust, and supernatural phenomena
6. Voice acting for key narrative moments and radio communications

## Best Practices
1. Build tension through pacing rather than constant action or jump scares
2. Create believable environments that enhance immersion and suspension of disbelief
3. Design enemy AI with unpredictable patterns that maintain player uncertainty
4. Balance resource scarcity to create tension without frustrating player progression
5. Implement multiple playthrough incentives with branching narratives and endings
6. Ensure accessibility options for players with different comfort levels with horror

## Common Pitfalls
1. Overusing jump scares leading to desensitization and reduced effectiveness
2. Poor pacing that either rushes or drags the horror experience
3. Predictable enemy behavior that removes tension and uncertainty
4. Inadequate atmosphere failing to create genuine unease or dread
5. Repetitive gameplay mechanics that become monotonous over time
6. Neglecting accessibility for players with different sensitivities to horror content

## References
1. [Horror Game Design Principles](https://www.gamedevelopment.net/horror-game-design)
2. [Atmospheric Tension Techniques](https://www.gamasutra.com/atmospheric-tension)
3. [Psychological Horror Mechanics](https://www.gamesindustry.biz/psychological-horror)