# Music World Template

## Overview
A template for creating music-based games with rhythm mechanics, song creation tools, and performance systems.

## Core Requirements
1. Rhythm mechanics with precise timing, note patterns, and musical progression
2. Song creation tools with composition, arrangement, and editing features
3. Performance systems with scoring, audience reactions, and career progression
4. Diverse instrument simulation with realistic sound and play mechanics
5. Social features with sharing, collaboration, and community content
6. Visual presentation systems with stage shows, animations, and effects

## Recommended Structure
```
music-world/
├── assets/
│   ├── instruments/
│   ├── songs/
│   ├── visuals/
│   └── ui/
├── src/
│   ├── core/
│   │   ├── rhythm_system.py
│   │   ├── song_editor.py
│   │   └── performance.py
│   ├── entities/
│   │   ├── instrument.py
│   │   ├── song.py
│   │   └── performer.py
│   ├── systems/
│   │   ├── audio.py
│   │   ├── scoring.py
│   │   └── social.py
│   └── ui/
│       ├── editor.py
│       ├── performance_ui.py
│       └── social_feed.py
├── data/
│   ├── instruments.json
│   ├── songs.json
│   └── performances.json
└── README.md
```

## Essential Systems
1. **Rhythm System** - Manages precise timing, note patterns, and musical progression
2. **Song Editor** - Handles composition, arrangement, and editing features
3. **Performance System** - Coordinates scoring, audience reactions, and career progression
4. **Audio System** - Implements instrument simulation and sound mixing
5. **Scoring System** - Tracks performance metrics, achievements, and rankings
6. **Social System** - Manages content sharing, collaboration, and community features

## Assets Required
1. Instrument visuals with playable interfaces and realistic designs
2. Audio samples for instruments, effects, and musical elements
3. Visual effects for performances, stage shows, and audience reactions
4. UI elements for editors, performance displays, and social features
5. Animation sets for performers, avatars, and stage elements
6. Background art for venues, studios, and performance spaces

## Best Practices
1. Design intuitive interfaces for both playing and creating music content
2. Provide clear visual and audio feedback for rhythm gameplay
3. Create robust editing tools that are accessible to beginners but powerful for experts
4. Implement fair scoring systems that reward skill and creativity
5. Support various input methods including controllers, keyboards, and specialized devices
6. Ensure accessibility options for players with different musical abilities

## Common Pitfalls
1. Creating overly complex editors that intimidate rather than inspire creativity
2. Poor timing detection leading to unfair judgments in rhythm gameplay
3. Inadequate tutorial systems leaving players confused about core mechanics
4. Repetitive content lacking variety in instruments, songs, or gameplay modes
5. Neglecting social features that could enhance community engagement
6. Ignoring accessibility for players with different physical abilities or musical knowledge

## References
1. [Music Game Design](https://www.gamedevelopment.net/music-game-design)
2. [Rhythm Mechanics](https://www.gamasutra.com/rhythm-mechanics)
3. [Creative Tools in Games](https://www.gamesindustry.biz/creative-tools-games)