# ITI Mission Control — prototype specification v0.1

Status: design/prototype branch, not released.

## Camera
- First-person walk view
- Third-person follow camera
- Top-down tactical dispatch camera
- Camera cycle via V or controller Y, with transition interpolation and camera collision work later
- Preserve player and world state across views

## Prototype gameplay
- Earth outpost, solar array repair, deploy from Mission Control
- WASD/left stick movement, mouse/right stick look
- Controller A to interact, X to open multitool, Start for dashboard
- Haptics best-effort only
- Local auto-save and JSON export/import
- Level 1 of 10-story campaign; later lunar grid dispatch, finite deposits, ice extraction and propellant production

## Quality targets
- Responsive camera and movement; smooth dashboard transition
- Grounded sci-fi visuals; coherent character, tool, vehicle, and structure assets
- Lightweight HUD; no inventory-heavy design
- Optional US flag default and other national flags; ITI insignia from research library
- Offline-first playable build, without accounts
