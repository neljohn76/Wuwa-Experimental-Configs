Wuthering Waves v3.7 — LG V50S ThinQ — Three Profile Pack v2

Each profile folder includes:
- Engine.ini
- DeviceProfiles.ini
- GameUserSettings.ini

Requested profile label: Android_VeryHigh (no Android_SND855 custom profile).

IMPORTANT COMPATIBILITY NOTES
- These are experimental Unreal Engine-style templates, not verified against your exact installed v3.7 config schema.
- DeviceProfiles.ini syntax varies by UE version/game. Do not blindly replace the game's full DeviceProfiles.ini with the short template. Merge the section only if it matches the structure in your current file. If the game already has an [Android_VeryHigh DeviceProfile] section, merge the +CVars entries into that existing section instead of duplicating it.
- Engine.ini CVars may be ignored or overridden by game code.
- GameUserSettings.ini keys shown here are common Unreal settings, but Wuthering Waves may use other keys or rewrite them. Preserve your original file and merge carefully.
- The pack intentionally does not include AxManager tuning commands or spoof a GPU/device identity.
- Keep your currently working Frame Generation mechanism unchanged. The profile templates do not claim to enable it themselves.
- Before testing, back up the original Engine.ini, DeviceProfiles.ini, and GameUserSettings.ini.
- Apply one profile at a time. Test Balanced first, then Performance, then UltraVisuals. If you see a black screen, crashes, texture streaming problems, or worse stutter, restore the backups.
- Start with the in-game 60 FPS cap and compare the same route for 10 minutes per profile. Cooler helps with thermal headroom but cannot eliminate GPU/CPU bottlenecks.
