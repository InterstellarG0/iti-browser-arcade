# Mission Control — Loop Tuning v0.1

Goal: observe → detect → propose → test → compare → accept or rollback.

## Telemetry (local, opt-in)
- Frame time and FPS, camera transition duration, controller input latency (when measurable)
- Movement errors, stuck states, failed interactions, repair task completion, session crashes
- Record game version, device class, camera mode and timestamp; never capture private inputs or personal identifiers
- Export/import JSON log; local storage first, telemetry off by default

## Tuning graph
- Timeline of each measurable metric before/after change
- Annotate patch ID, baseline, candidate, test outcome, confidence and rollback
- Graph sample counts and separate different devices; never label an improvement from one noisy run

## Controlled automatic tuning
- Safe adjustments: graphics quality presets, shadow resolution, render scale, camera smoothing within bounded values, controller deadzone with user override
- Test candidate against baseline and quality limits; reject regressions; rollback if unstable
- Never silently rewrite executable code, deploy commits, upload telemetry or alter user preferences
- Code-level improvement proposals require review and explicit approval

## Acceptance criteria
- Toggle telemetry, view graph, inspect events, export logs
- Compare at least two runs; show insufficient-data state
- Revert last tuning change with one action
