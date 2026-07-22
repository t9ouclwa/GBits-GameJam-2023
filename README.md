# GBits GameJam 2023

A Unity horizontal action prototype created for a 48-hour game jam by a two-person team.

This repository contains the recovered Unity project files from the `HorizontalAction` archive. The documentation is written for portfolio review while avoiding unverified claims about awards, team roles, or final event ranking.

## 48-Hour Game Jam

This project was developed under a 48-hour game jam constraint. The source project shows a compact Unity prototype focused on movement, character interaction, simple enemy behavior, and a playable scene assembled with sample assets.

## Team

- Team size: Two-person team
- Engine: Unity
- Project name in recovered archive: `HorizontalAction`

## Gameplay

The project is a side-view horizontal action prototype.

Observed gameplay elements from the source files:

- Horizontal player movement
- Jumping with grounded-state checks
- Character rotation based on movement direction
- Grab-and-release interaction for objects tagged as `GrabBox`
- Stomp-style damage detection using downward raycasts
- Simple AI movement that periodically chooses random horizontal input and jump behavior
- Camera follow behavior for the player character

## Controls

Based on `Assets/Gameplay/Scripts/PlayerController.cs`:

- Move: horizontal input axis
- Jump: `Space`
- Grab / release object: `G`

## Technologies

- Unity `5.6.0f3`
- C#
- Unity `CharacterController`
- Unity Animator Controller
- Unity prefabs, materials, audio, textures, and sample assets

## Source Structure

```text
GBits-GameJam-2023/
├── Assets/
│   ├── Game.unity
│   ├── Gameplay/
│   │   ├── Animator/
│   │   ├── Prefabs/
│   │   └── Scripts/
│   └── SampleAssets/
├── ProjectSettings/
├── docs/
│   └── screenshots/
├── .gitignore
├── LICENSE
└── README.md
```

Key scripts:

- `Character.cs` - shared movement, jumping, damage, death, gravity, animation state, and attack detection
- `PlayerController.cs` - player input handling
- `PlayerCharacter.cs` - player-specific grab and release behavior
- `AIController.cs` - simple randomized AI movement and jumping
- `PlayerCamera.cs` - player-following camera behavior

## My Responsibilities

The exact personal task split should be confirmed before using this section in an application. Based on the recovered source structure, the project includes work areas that can be described after confirmation:

- Gameplay programming for character movement and jumping
- Object interaction design for grabbing and releasing boxes
- AI behavior scripting for simple enemy movement
- Scene assembly using Unity prefabs, materials, audio, and sample assets
- Game jam debugging and final prototype preparation

## Completion Award

The original work order notes that this project received a completion award. Add the official award name, certificate, or event page link here when available.

## Screenshots

Add redacted project screenshots to [`docs/screenshots`](docs/screenshots).

Suggested screenshots:

- Main gameplay scene
- Player movement or jumping
- Grab interaction with a box
- AI character behavior
- Completion award or certificate, if available

## Notes for Portfolio Review

- This repository includes source project files, not only documentation.
- Generated Unity folders such as `Library/`, `Temp/`, `Obj/`, and build outputs are intentionally ignored.
- The original `.unitypackage` archive was not committed because the expanded Unity project is already present and easier to inspect.

## License

Project-specific code is licensed under the MIT License. See [`LICENSE`](LICENSE) for details. Third-party or sample assets may be subject to their original licenses.
