<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/34c4347a-3253-4d4f-a199-e73c3f79adcb" />

# crDroid 12.11 QPR2 | Stable | Signed | OFFICIAL 

### Realme 8i / Narzo 50 (`spaced`)
### Android 16  
### Maintained by **DΞΞZNUTZ**

---

# 🚀 Release Changelog — July 03, 2026

### 📺 Display & Performance
* **Flicker Fix:** Resolved intermittent screen flickering issues occurring during HWC overlay composition.
* **Pipeline Tuning:** Improved `SurfaceFlinger` and display pipeline tuning for better frame pacing.
* **Phase Offsets:** Imported optimized phase offsets from Motorola to achieve significantly smoother rendering.
* **UI Responsiveness:** Tuned HWUI caches specifically for Mali-G57 to ensure much smoother rendering.
* **120Hz Optimization:** Shortened activity transition animations to **100ms** for a snappier, more fluid high-refresh-rate feel.

### ⚙️ System, Memory & Power
* **Powerhint Correction:** Fixed `powerhint` frequency values to accurately match the actual hardware OPP (Operating Performance Points) table.
* **ZRAM Efficiency:** Switched default ZRAM compression algorithm to **ZSTD** for superior memory efficiency and compressed throughput.
* **Storage Modernization:** Removed legacy `SDCARD_FS` driver kernel-side in favor of modern **FUSE** emulation.
* **Storage Tuning:** Optimized I/O scheduler and read-ahead values for both UFS and eMMC chips to elevate storage performance.
* **Battery Stats Preservation:** Added `wakelock` and `input` groups to `fuelgauged` so battery statistics keep working flawlessly through system suspend.

### 🔒 SELinux & Security
* **Denial Fixes:** Addressed critical SELinux denials by explicitly granting `system_suspend` and `system_server` permissions to access required vendor nodes.
* **Policy Cleanups:** Dropped unused and redundant rules inside `system_server_ext.te`.

### 🛠️ Kernel & Device Trees
* **Compilation Fix:** Resolved a `zsmalloc` `rwlock` compilation error on specific build configurations.
* **Log Cleanups:** Downgraded a highly noisy GPU clock speed warning to debug-only (`pr_debug`) to reduce log spam.
* **WLAN Handling:** Cleaned up and streamlined fallback handling routines for WLAN firmware loading.

### 🎵 Multimedia & Audio
* **Audio Expansion:** Integrated official **Sony Dolby** audio support.
* **Audio FX:** Enabled full **Dolby AudioFX** backend support and effects processing.

---

### ⚠️ Notes
* Clean flash recommended
* Dirty flash from previous crDroid builds may work but is not guaranteed

---

### 📝 **Notes & Installation**
* A clean flash is highly recommended if migrating from another ROM.

### 🤝 **Credits & Thanks**
* Huge thanks to `@HELLINFIX` for the foundational source collaboration and device tree support.
* Thanks to `@ViaanLarryROMS` for the assistance in adding Sony Dolby.
* Thanks to `@hxfuxyy` for teaching me how to implement OTA updates.

---

### 🤝🏻 **Buy me a coffee?**
* Github Sponsor: [**Sponsor**](https://github.com/sponsors/daizeuz-dred)
* Sociabuzz: [**Sponsor**](https://sociabuzz.com/daizeuzdred/tribe)

---
