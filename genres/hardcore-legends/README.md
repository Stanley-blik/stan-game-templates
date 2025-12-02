# Hardcore Legends Template

## Overview
A template for creating challenging games with demanding mechanics, permadeath elements, and skill-based progression systems.

## Core Requirements
1. Challenging gameplay mechanics requiring mastery and precise execution
2. Permadeath or significant consequence systems for player actions
3. Skill-based progression with meaningful improvement over repeated attempts
4. Balanced difficulty that encourages learning rather than frustration
5. Clear feedback systems for understanding failure causes
6. Reward structures that acknowledge effort and incremental improvement

## Recommended Structure
```
hardcore-legends/
├── assets/
│   ├── characters/
│   ├── environments/
│   ├── ui/
│   └── effects/
├── src/
│   ├── core/
│   │   ├── challenge_manager.py
│   │   ├── progression.py
│   │   └── consequence_system.py
│   ├── entities/
│   │   ├── player.py
│   │   ├── enemy.py
│   │   └── hazard.py
│   ├── systems/
│   │   ├── combat.py
│   │   ├── skill_check.py
│   │   └── feedback.py
│   └── ui/
│       ├── hud.py
│       ├── death_screen.py
│       └── progression_display.py
├── data/
│   ├── challenges.json
│   ├── progression.json
│   └── rewards.json
└── README.md
```

## Essential Systems
1. **Challenge Management System** - Designs and implements demanding gameplay scenarios
2. **Consequence System** - Handles permadeath, penalties, and significant failure outcomes
3. **Skill Progression** - Tracks player improvement and unlocks new capabilities
4. **Feedback System** - Provides clear information about performance and failure causes
5. **Reward System** - Acknowledges effort and achievement despite failures
6. **Adaptive Difficulty** - Adjusts challenge based on player performance and skill

## Assets Required
1. Character sprites or models with clear visual states for health, status, and actions
2. Environmental art that creates challenging scenarios and hazardous situations
3. UI elements for displaying critical information without cluttering gameplay
4. Visual effects for hits, deaths, and important gameplay moments
5. Sound effects that clearly communicate danger, success, and failure
6. Music tracks that intensify during challenging moments and provide emotional payoff

## Best Practices
1. Design fair but challenging scenarios that test skill rather than luck
2. Provide clear visual and audio feedback for all critical gameplay events
3. Create meaningful progression that persists despite character deaths
4. Balance difficulty to encourage learning rather than pure repetition
5. Implement tutorial systems that prepare players for hardcore challenges
6. Ensure accessibility options for players with different skill levels and abilities

## Common Pitfalls
1. Making challenges feel arbitrary or based on luck rather than skill
2. Providing inadequate feedback leading to confusion about failure causes
3. Creating overly punishing consequences that discourage continued play
4. Poor progression systems that don't acknowledge player improvement
5. Neglecting accessibility for players with different physical abilities
6. Balancing difficulty too harshly, causing frustration rather than engagement

## References
1. [Hardcore Game Design Principles](https://www.gamedevelopment.net/hardcore-game-design)
2. [Permadeath Mechanics](https://www.gamasutra.com/permadeath-game-design)
3. [Skill-Based Progression Systems](https://www.gamesindustry.biz/skill-progression-systems)