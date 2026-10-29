# Wuthering Waves v3.7 — Snapdragon 855 Mengzhou Profile v1.1

## Files
- `Engine.ini`: mergeable `[SystemSettings]` tuning section.
- `DeviceProfiles.ini`: optional experimental device profile.

## Intended balance
- Lower SSR, shadows, ambient occlusion, refraction, and selected post-processing costs.
- Preserve anisotropic texture filtering and avoid an aggressively positive mip bias.
- No forced FPS, resolution, Vulkan, or memory-pool override.

## Installation
1. Back up your current config files.
2. Merge the `[SystemSettings]` section from `Engine.ini` into the existing Engine.ini. Do not delete existing sections such as `[Core.System]`.
3. Only merge the device profile if your game build reads this file and the profile hierarchy is compatible. Do not create duplicate profile names.
4. Test in Mengzhou for 10–15 minutes, including traversal and combat. Compare frame pacing and temperatures, not just peak FPS.
5. If shadows or effects break, remove the related CVars first.

## Accuracy and limitations
This is an experimental tuning patch, not an official or verified Kuro v3.7 preset. The exact active config schema and CVar support can differ by game build. Some entries may be ignored or overridden by the game. The patch cannot eliminate shader-compilation or asset-streaming stutter and does not guarantee a particular FPS.

Recommended in-game starting point: 30 FPS cap, medium resolution, low-to-medium shadows, medium effects, high character detail where available.
