# STRIKER ZERO — Unreal Engine 5 Starter Prototype

An original anime-inspired football prototype. This is a source starter project, not a compiled game. It contains a controllable third-person player, physics football, kick/pass controls, a procedural greybox pitch, goal triggers, a simple score/time HUD, sprint and a camera-distance toggle.

## Engine compatibility

The project descriptor targets Unreal Engine 5.4. Open with UE 5.4 if available. If using a newer UE5 release, allow Unreal to update the project when prompted. The C++ source uses the standard Unreal Build Tool workflow.

## Open the project

1. Extract the entire `STRIKER_ZERO` folder.
2. Right-click `STRIKER_ZERO.uproject` and choose **Generate Visual Studio project files** (or open the `.uproject` and let Unreal generate project files).
3. Open `STRIKER_ZERO.sln` in Visual Studio with the **Game development with C++** workload installed.
4. Build the `STRIKER_ZEROEditor` target in Development Editor / Win64.
5. Open the `.uproject` in Unreal Editor and press Play.

If the project opens without compiling, use **Tools → Refresh Visual Studio Project** or regenerate project files.

## Controls

- WASD — move
- Mouse — rotate/look
- Left Shift — sprint
- Left mouse button — shoot when close to the ball
- Space — pass when close to the ball
- C — toggle between close player camera and wider elevated camera

The prototype currently starts a five-minute match timer and tracks goals. It is a foundation, not a complete 22-player match yet: team AI, goalkeeper AI, formations, full rules, custom anime characters, cinematic ability animations and multiplayer are future milestones.

## Important implementation note

The pitch, goal frames, ball and goal triggers are spawned at runtime by the game mode, so no pre-authored map is required for the initial test. The visual geometry is intentionally simple greybox geometry. Replace it with original/licensed art as development progresses.

## Next milestone

Add a second controllable/AI player, then basic teammate and opponent AI. Only after the ball feel and match loop are reliable should the project expand to full 11 vs 11.
