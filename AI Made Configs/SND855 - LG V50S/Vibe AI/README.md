# 🤖 Vibe AI Config Family — WuWa v3.7 (Lahai Roi)

Three ready-to-install tiers for the **LG V50S ThinQ 5G** (Snapdragon 855 / Adreno 640, 60 Hz OLED), built from scratch with **Vibe AI** — not based on Arglax's Mobile-WuWa-Config files.

Every tier is a complete 3-file set (`DeviceProfiles.ini` + `Engine.ini` + `GameUserSettings.ini`) using the modern v3.6+ pattern: `dp.Override=Android_High` + `DeviceScore=6969`, with **zero** ConfigMonitor-blacklisted CVars.

## 🎛️ Pick your tier

| | **Performance** | **Balanced** | **Visual** |
|---|---|---|---|
| Goal | Locked 60 FPS, cool & quiet | Daily driver: smooth **and** pretty | Near-PC showcase |
| sg.ShadowQuality | 2 | 3 | 3 |
| sg.TextureQuality | 3 | 4 | 4 |
| sg.AntiAliasingQuality | 1 | 2 | 2 |
| sg.FoliageQuality | 1 | 2 | 2 |
| Per-object shadows | 128 px | 256 px | 256 px + point-light shadows |
| SSR / water reflections | ❌ | ✅ | ✅ (extended roughness) |
| Light shafts | ❌ | ✅ | ✅ + Tyndall scattering |
| Volumetric clouds | ❌ | ✅ | ✅ |
| Motion blur / DOF | ❌ | ❌ | ✅ |
| Foliage density / far cull | 0.7 / 7000 | 0.9 / 8500 | 1.0 / 10000 |
| Grass cull | 1500 | 2200 | 2800 |
| Anisotropy | 4× | 8× | 16× |
| Streaming range (`wp.Runtime`) | 0.45 / 0.60 | 0.55 / 0.75 | 0.70 / 0.85 |
| Expected thermals | Low | Medium | High — use cooling |

All tiers keep: `t.MaxFPS=60`, anti-battery-throttle flags, GC/async-streaming tuning, PSO shader-cache warming, Vulkan Adreno-640 flags, and the **sg.EffectsQuality=2 crash guard** (3+ crashes the game on Adreno 640 — never raise it).

## 📲 Install

Back up your current files, then copy **all three** files from your chosen tier folder to:

```
Android/data/com.kurogame.wutheringwaves.global/files/UE4Game/Client/Client/Saved/Config/Android/
```

Overwrite when prompted. After a patch, expect one long traversal of stutter while the shader cache rebuilds.

## ⚠️ Notes

- Each file's header documents tuned fallbacks — apply those instead of blindly lowering values.
- Verify via your decrypted `Client.log` that CVars actually apply after each WuWa update.

## 👤 Credits

Config by **Nel John Acosta** — part of the LG V50S Experimental Config Project. Built with Vibe AI.
