FRAME GENERATION — separate compatibility note

Do not assume the Snapdragon 855 supports Wuthering Waves' official mobile Frame Generation in v3.7. The official patch notes do not list it as supported.

The pack intentionally does not include a DeviceProfiles.ini GPU spoof. A spoof can make an option appear without making the rendering path compatible. First test the three stable rendering profiles. Only experiment with community device-profile overrides if you accept possible crashes, visual artifacts, or the need to restore the original file.

If Frame Generation is already available in the game's own Graphics menu, test it separately with the Balanced profile and compare frame pacing, latency, artifacts, and temperature. If it is absent, these Engine.ini profiles cannot reliably enable it.
