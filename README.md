<!-- Banner -->
<p align="center">
  <img src="assets/banner.png" alt="Unreal Vulkan Config Banner" width="800"/>
</p>

<h1 align="center">⚙️ UE4 Wuthering Waves Vulkan Config Collection (v2.7+)</h1>
<p align="center">
  <em>Experimental configurations tuned for Vulkan API performance, reflection quality, and smooth gameplay across major Android chipsets.</em>
</p>

---

<p align="center">
  <a href="#"><img src="https://img.shields.io/badge/API-Vulkan-blue?style=for-the-badge&logo=vulkan" alt="Vulkan API"></a>
  <a href="#"><img src="https://img.shields.io/badge/Status-Experimental-orange?style=for-the-badge" alt="Status"></a>
  <a href="#"><img src="https://img.shields.io/badge/Version-v3.7%20%2B%20v2.7-success?style=for-the-badge" alt="Version"></a>
</p>

---

## 🌍 Overview
These configs fine-tune Unreal Engine rendering for Vulkan-capable Android devices — pushing higher reflections, better shadow accuracy, and GPU-optimized thread handling.  
Each config is customized per chipset to get the most stable performance possible without losing that high-fidelity look.

> 🆕 **October 2026:** Added a **v3.7 build for the Lahai Roi update** (Qualcomm/Adreno mid-tier) in [`Qualcomm Config v3.7/`](./Qualcomm%20Config%20v3.7). It removes CVars that Kuro now blacklists at runtime and uses the modern `dp.Override` + `DeviceScore` profile pattern. The v2.7 configs are kept for reference but are **not recommended on 3.7+**.

---

## 🧩 Configurations

| Chipset | Folder | Vulkan Support | Description |
|----------|---------|----------------|--------------|
| 🔵 Qualcomm **v3.7** ⭐ | [`Qualcomm Config v3.7/`](./Qualcomm%20Config%20v3.7) | ✅ Native | **New** — v3.7 Lahai Roi build, mid-tier Adreno, modern profile pattern |
| 🔵 Qualcomm (v2.7) | [`Qualcomm/`](./Qualcomm%20Config) | ✅ Forced | Legacy — optimized for **Adreno GPUs**, pre-3.1 CVars (partially blacklisted now) |
| 🔹 Exynos (v2.7) | [`Exynos/`](./Exynos%20Config) | ✅ Forced | Refined Vulkan config for **Mali GPUs** — clean lighting, minimal stutter |
| 🔸 MediaTek (v2.7) | [`MediaTek/`](./MediaTek%20Config) | ✅ Native | Stable Vulkan config for **Dimensity / Helio** chips |
| ⚫ Universal (v2.7) | [`Universal/`](./Universal%20Config) | ✅ Auto | Balanced setup for all Vulkan-supported devices |

---

## ⚠️ Warnings

> ⚠️ **Always back up** your existing config files before replacing them.  
> These are *experimental configs* that can cause issues if your device or UE version handles Vulkan differently.

**Backup Path Example:**

Android/data/com.kurogame.wutheringwaves/files/UE4Game/Client
/Client/Saved/Config/Android/

---

## 💡 Tips
- Use **Performance Mode** before launching the game.  
- If the game fails to boot, delete the `.ini` and restore your backup.  
- Pair Vulkan configs with proper **thermal management apps** for best stability.  
- Ideal for testing in **Wuthering Waves**, **Tower of Fantasy**, **PUBG UE**, and other Vulkan-based titles.

---

## 🧠 Version Info
- **Engine:** Unreal Engine 4 / 5  
- **API:** Vulkan  
- **Config Version:** v2.7 (Qualcomm v3.7 build added for the 3.7 Lahai Roi update)  
- **Status:** Experimental  
- **Last Updated:** 2026-10-17  

---

## 👤 Credits
Created by **Nel**  
Inspired by **Kuro's Config Type (v2.7+)** and the **LG V50S Experimental Config Project**  
v3.7 build based on tested stable configs from **Arglax / Mobile-WuWa-Config**

> 🧩 “Vulkan runs deep — reflections, frames, and the fire beneath your GPU.”
