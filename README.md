<div align="center">

# ⚙️ WuWa Experimental Configs

**Hand-tuned Unreal Engine configs for Wuthering Waves on Android — built device-by-device, not one-size-fits-all.**

[![WuWa Version](https://img.shields.io/badge/Game-WuWa%20v3.7%20%7C%20Lahai%20Roi-7b5cff?style=flat-square)](https://wutheringwaves.kurogames.com)
[![Engine](https://img.shields.io/badge/Engine-UE4.27%20%2B%20Vulkan-2563eb?style=flat-square)](https://www.unrealengine.com)
[![Status](https://img.shields.io/badge/Status-Experimental-f97316?style=flat-square)](./README.md#warningy-read-first)
![Made with](https://img.shields.io/badge/Made%20by-Nel%20John%20Acosta-10b981?style=flat-square)

</div>

---

> 🆕 **October 2026 — updated for WuWa v3.7 (Lahai Roi).**
> New: the **AI Made Configs** collection (ChatGPT / Claude / Mistral / Vibe generations for the LG V50S) and the maintained **Vibe AI tier family** — Performance, Balanced, Visual. The old v2.7 Vulkan configs remain as legacy reference and are **not recommended on 3.7+**.

---

## 🎛️ Choose your config

### ⭐ Vibe AI tier family — `AI Made Configs/SND855 - LG V50S/Vibe AI/`

The current, maintained configs for the **LG V50S ThinQ** (SD855 / Adreno 640). Complete 3-file sets, zero blacklisted CVars, tuned fallbacks documented in every header.

| Tier | Best for | Look | Load |
|---|---|---|---|
| 🚀 **Performance** | Locked 60 FPS, long sessions, hot weather | Clean but stripped | Lightest |
| ⚖️ **Balanced** | Daily driver — smooth *and* pretty | Shadows, water reflections, light shafts, volume clouds | Medium |
| 💎 **Visual** | Near-PC showcase | + motion blur, DOF, Tyndall god rays, point-light shadows, PC foliage density | Heaviest |

→ Full comparison table in the [Vibe AI README](./AI%20Made%20Configs/SND855%20-%20LG%20V50S/Vibe%20AI/README.md).

### 📦 Other config families

| Folder | Description | Status |
|---|---|---|
| `Qualcomm Config v3.7/` | Balanced-Visual+ v2.0 — Adreno mid-tier build for v3.7 | ✅ Current |
| `AI Made Configs/` | Multi-AI config generations for the LG V50S (reference + comparison) | ✅ Current |
| `Qualcomm Config/` · `MediaTek Config/` · `Exynos Config/` · `Universal Config/` | v2.7-era Vulkan experiments | ⚠️ Legacy |

---

## 📲 Install (manual)

1. Back up your current `.ini` files first.
2. Copy **all three** files from your chosen tier (`DeviceProfiles.ini`, `Engine.ini`, `GameUserSettings.ini`) to:

```
Android/data/com.kurogame.wutheringwaves.global/files/UE4Game/Client/Client/Saved/Config/Android/
```

3. Overwrite when prompted, then launch the game.
4. After a WuWa patch, do one long traversal to rebuild the shader cache before judging smoothness.

> 💡 Keep the in-game resolution scale at ~72–80% on 1440p LG panels — the game renders internally at its mobile scale regardless.

---

## ⚠️🆕 Read first

- **sg.EffectsQuality=2 is a hard cap.** 3+ crashes the game on Adreno 640.
- **Kuro's ConfigMonitor blacklists ~50 CVars** (`r.Streaming.PoolSize`, `r.Shadow.MaxResolution`, `r.ViewDistanceScale`, `r.ScreenPercentage`, `r.MaterialQualityLevel`, `r.KuroFI.Enable`, `r.Mobile.DeviceEvaluation`, …). They are stripped at runtime and do nothing — all configs in this repo avoid them.
- Every config is **experimental**: back up, test, and check your decrypted `Client.log` after game updates.
- If a config misbehaves, delete the `.ini` files and let the game regenerate defaults.

---

## 📜 Version history

| Date | Change |
|---|---|
| **Oct 2026** | WuWa v3.7 (Lahai Roi) support: Vibe AI tier family (Performance / Balanced / Visual), AI Made Configs collection, modern `dp.Override` + `DeviceScore` profile pattern, all blacklisted CVars removed |
| Oct 2026 | `Qualcomm Config v3.7/` — Balanced-Visual+ v2.0 (Adreno mid-tier) |
| Oct 2025 | v2.7 Vulkan config wave — Qualcomm / MediaTek / Exynos / Universal (now legacy) |

---

## 🙏 Credits & License

Created and maintained by **NelJohn 76** — part of the **LG V50S Experimental Config Project**.
The Vibe AI config family was built with [Vibe](https://chat.mistral.ai) (GLM) on Nel's behalf.

> **Disclaimer** — these configurations are provided "as is", without warranty of any kind. Experimental config users have been around a long time, but still: *use at your own risk.* Kuro's ConfigMonitor may change behavior in any patch. If Kuro Games requests removal of config tooling or files, they will be taken down.

<div align="center">

*“Vulkan runs deep — reflections, frames, and the fire beneath your GPU.”*

</div>
