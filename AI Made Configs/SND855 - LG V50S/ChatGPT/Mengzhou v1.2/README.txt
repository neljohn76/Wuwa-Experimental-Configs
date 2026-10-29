Wuthering Waves v3.7 — Snapdragon 855 Mengzhou Experimental v1.2

Files:
- Engine.ini: includes the recovered [Core.System] plugin-path block plus tuning sections.
- DeviceProfiles.ini: includes AndroidDeviceProfile and Snapdragon/Adreno profile mappings.
- README.txt: installation notes.

Important:
1. This update restores the missing Core.System paths and device-profile structure based on your saved v3.7 baseline.
2. These are experimental values. Profile names and accepted CVars depend on the game's build and configuration loader.
3. Keep a backup. If your config manager expects the original split between DEFAULT and COMMUNITY sections, preserve that structure rather than replacing the whole combined file.
4. Check that your loader accepts +CVars syntax in DeviceProfiles.ini. Some Unreal profile files use CVars= entries instead; follow the syntax of your working baseline.
5. Vulkan is not forced by this pack. The Android Vulkan-related settings only preserve the prior baseline's enablement.
6. Test Mengzhou traversal and combat. Remove the device-profile override first if settings appear ignored or cause rendering issues.
