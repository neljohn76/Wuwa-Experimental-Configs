# 🔵 Qualcomm Config v3.7 — Balanced-Visual+ (Adreno Mid-Tier)

> Successor to the v2.7 Qualcomm config, rebuilt for **Wuthering Waves v3.7 (Lahai Roi)**.
> Stable frame pacing in the new region + noticeably better visuals than the old build.

---

## ⚙️ What changed vs v2.7

- **Removed CVars blacklisted by Kuro's ConfigMonitor** (they get stripped at runtime and do nothing since ~3.1): `r.Streaming.PoolSize`, `r.Shadow.MaxResolution`, `r.Shadow.DistanceScale`, `r.KuroFI.Enable`, `r.Mobile.DeviceEvaluation`, `r.ScreenPercentage`, and more.
- **sg.EffectsQuality capped at 2** — level 3+ crashes the game.
- **Removed desktop-only CVars** that never applied on mobile UE4.27: `r.GraphicsRHI`, `r.Lumen.*`, `r.Vulkan.PresentMode`, `r.DisplayRefreshRate`, `r.AllowHDR`, `r.FullScreenMode`, etc.
- **Modern profile pattern (v3.6+):** `dp.Override=Android_High` + `DeviceScore=6969` instead of the old `DeviceProfileNameAndTypes` block that never actually matched.
- **Lahai Roi tuning:** `wp.Runtime.LoadingRangeScale=0.55` / `PlannedLoadingRangeScale=0.75`, capped Kuro foliage cull distances (8500 far / 2200 grass), async FX tick, PSO shader pipeline caching.
- **Visuals up vs v2.7:** 256px per-object shadows with 2 CSM cascades, scene-object SSR + water SSR, bloom + light shafts + volume clouds, 8x anisotropy, translucency lighting dim 32, scene color format 4.

---

## 📱 Ideal devices

LG V50S/V50 • Snapdragon 855/865/870 • Snapdragon 778G / 7 Gen 1 — anything **Adreno 640-class and up**.

> For 60Hz panels, keep VSync on (this config sets it) and use an in-game resolution of ~72–80% rather than native.

---

## 💾 Install

Back up your current files, then copy `Engine.ini` and `DeviceProfiles.ini` to:

```text
Android/data/com.kurogame.wutheringwaves.global/files/UE4Game/Client/Client/Saved/Config/Android/
```

Overwrite when prompted. On first launch, do one long traversal in Lahai Roi to warm the shader cache before judging smoothness.

---

## 🙏 Credits

- Base: **Arglax / Mobile-WuWa-Config** (v3.7.3-tested Stable Mid-End) — also the source for the forbidden-CVars blacklist.
- Config by **Nel** — part of the LG V50S Experimental Config Project.
