<div align="center">

# ⚡ PeerDrop Pro v4.2 — Universal Adaptive P2P Stream Engine
### **Uncompressed 4K/8K Video & 100GB+ File Transfer • WhatsApp-Style P2P Chat Room • Mobile Quota Shield**

[![Release](https://img.shields.io/badge/Release-v4.2_Universal-00a884?style=for-the-badge)](./PeerDrop-v4.2-Windows-x64.zip)
[![Adaptive Engine](https://img.shields.io/badge/Adaptive_Pacing-16_Mbps_ADSL_%E2%86%94_1000_Mbps_Fiber-f59e0b?style=for-the-badge)](#2-universal-adaptive-gear-engine-bbr-style-anti-bufferbloat)
[![Security](https://img.shields.io/badge/Cryptography-SHA256_%2B_Ed25519-38bdf8?style=for-the-badge)](#6-cryptographic-security--ed25519-pro-licensing)
[![i18n](https://img.shields.io/badge/Auto_Region_UI-EN_%7C_TR_%7C_DE_%7C_RU_%7C_ES_%7C_FR-8b5cf6?style=for-the-badge)](#5-auto-region-multi-language-engine-6-languages)

**Zero Cloud Storage Cost • No Receiver App Required • Local Gigabit Wi-Fi & Global Cloudflare HTTP/2 Tunnel**

[📥 **Download Windows x64 Portable (.zip)**](./PeerDrop-v4.2-Windows-x64.zip) • [🚀 **How It Works**](#1-ultra-fast-4k8k-video--100gb-streaming-architecture) • [📊 **Benchmarks & Comparison**](#-why-peerdrop-pro-competitor-comparison)

</div>

---

## 🌐 Overview

**PeerDrop Pro v4.2** is a high-performance, self-hosted P2P file streaming engine and persistent WhatsApp-style chat room designed to transfer **uncompressed 4K/8K videos, raw camera footage, and 100GB+ archives** directly between PCs and smartphones (iOS / Android) with **zero cloud storage costs**.

**Receivers do not need to install any app or create an account.** Share a single link via WhatsApp/Telegram or scan a QR code—the recipient connects directly to your node through their mobile/desktop browser over local Gigabit LAN or a global Cloudflare HTTP/2 tunnel.

---

## 📊 Why PeerDrop Pro? (Competitor Comparison)

| Feature | ⚡ **PeerDrop Pro v4.2** | **Blip** | **LocalSend** | **SendAnywhere** | **WhatsApp / Telegram** |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **App Required for Receiver** | **No (Works in Browser via Link/QR)** | Mandatory (App + Account) | Mandatory | No (Ad-heavy) | Mandatory |
| **Works Across Different Networks (4G/5G / WAN)** | **Yes (Global Cloudflare HTTP/2 Tunnel)** | Yes | **No (Same Wi-Fi Only)** | Yes (Quota Limited) | Yes |
| **Persistent Two-Way Chat & Clipboard Room** | **Yes (WhatsApp-Style Timeline)** | No | No | No | Yes |
| **Video Compression & Size Limit** | **Zero Compression / Unlimited (100GB+)** | Unlimited | Unlimited | Limited on Free | **2GB–4GB Limit & Heavy Compression** |
| **Mobile Data Quota Shield & Wi-Fi Queue** | **Yes (Auto-Queue Until Wi-Fi)** | No | No | No | No |
| **16 Mbps ADSL ↔ 1000 Mbps Adaptive Pacing** | **Yes (64 KB Paced ↔ 4 MB Turbo Blocks)** | Partial | Static | Static | Static |

---

## 🔥 Core Engineering Features

### 1. Ultra-Fast 4K/8K Video & 100GB+ Streaming Architecture
Standard web browsers crash when transferring multi-gigabyte videos because they attempt to buffer the entire file in RAM (`Blob`). **PeerDrop Pro v4.2** eliminates memory bottlenecks using **Direct Atomic Disk Streaming (`WriteAt` + `.part` Isolation)**:

* **100% Lossless Original Quality:** Raw `.mp4`, `.mov`, and `.mkv` 4K/8K videos stream directly to disk without re-encoding or quality loss.
* **Atomic `.part` Shield (Zero `0 KB` Corrupted Files):** Incoming streams are written to isolated `.part` files and are only promoted to the chat timeline after 100% completion and **end-to-end SHA-256 verification**.
* **Gigabit Local Wi-Fi Speeds (50–100+ MB/s):** When devices share the same router, traffic bypasses the external internet completely for maximum hardware throughput.
* **Drag & Drop, Clipboard Paste (`Ctrl+V`), and Multi-File Queue:** Drop multiple videos or files directly into the chat window or paste screenshots instantaneously.

---

### 2. Universal Adaptive Gear Engine (BBR-Style Anti-Bufferbloat)
Pushing large packets over a slow connection (such as 16 Mbps ADSL with 0.8 Mbps upload, or weak 2-bar cellular 4G) floods the router's uplink buffer (**Bufferbloat**), causing tunnel disconnects (`Error 1033`) and timeouts.

**PeerDrop Pro v4.2** measures per-chunk throughput in real time and dynamically adjusts both **chunk size** and **inter-packet pacing delay**:

| Network Condition | Measured Instant Speed | Automatic Gear (Chunk Size) | Anti-Bufferbloat Pacing | Engineering Result |
| :--- | :--- | :--- | :--- | :--- |
| **Weak 4G / 16 Mbps ADSL** | `< 300 KB/s` | **`[ADSL/4.5G Safe 64KB]`** | **45 ms breathe window** | Never chokes the router uplink; zero tunnel drops (`Error 1033` prevented). |
| **Standard VDSL / 4G LTE** | `300 KB/s – 3 MB/s` | **`[VDSL/4.5G 512KB]`** | **15 ms pacing** | Smooth file transfer while keeping real-time chat messages responsive. |
| **High-Speed Fiber / 5G** | `3 MB/s – 15 MB/s` | **`[Fiber 2MB]`** | **0 ms** | Maximizes global Cloudflare HTTP/2 tunnel throughput. |
| **1000 Mbps Gigabit / Local Wi-Fi** | `> 15 MB/s` | **`[Gigabit Turbo 4MB]`** | **0 ms (Full Throttle)** | Transfers multi-gigabyte 4K videos in seconds. |

* **Motion-Sensor Watchdog (Stall-Only Timeout):** No rigid fixed timeouts. As long as bytes are moving—even on ultra-slow links—the transfer never aborts. If a network drop freezes traffic for 28 seconds, the engine automatically resumes from the exact byte offset (`Auto-Resume`).

---

### 3. Smart Mobile Data Quota Shield & Auto Wi-Fi Queue
Protects mobile users from accidentally burning through their cellular data plan when someone sends a massive video file:

* **🤖 Smart Ask Policy:** Automatically detects cellular connections and files larger than `20 MB`, displaying a red **`⚠️ MOBILE DATA QUOTA WARNING!`** with the exact MB/GB cost before downloading.
* **⏳ Queue Until Connected to Wi-Fi:** With one tap, mobile users can place large videos into the **Wi-Fi Waiting Queue**. Zero cellular data is used—queued files automatically begin downloading the moment the phone connects to a Wi-Fi network.
* **📱 Allow 4G/5G Override:** Instant bypass for urgent field transfers.

---

### 4. Zero-QR "Auto-Pass" Discovery (Anti-Error 1033 Beacon)
Free quick tunnels change their public URL whenever the host PC restarts. To eliminate rescanning QR codes every day:

1. **Permanent Room ID (`PD-XXX-XXX`) & Retained MQTT Beacon:** On startup, `peerdrop.exe` publishes its latest Cloudflare HTTP/2 tunnel URL and local LAN IP to a retained discovery topic tied to your Room ID.
2. **One-Tap Auto-Pass Launcher (`PeerDrop-PD-XXX-XXX.html`):** Download the 3 KB launcher file once via the **`📌 Auto-Pass`** button. Opening it on your phone automatically discovers your PC's newest tunnel URL in 1 second and redirects you straight into the chat room.
3. **Live Tab Auto-Recovery:** If a tunnel refreshes while the browser tab is open, the client automatically queries the beacon and migrates to the new tunnel URL without showing `Error 1033`.

---

### 5. Auto-Region Multi-Language Engine (6 Languages)
PeerDrop automatically detects the connecting device's **timezone (`Intl.DateTimeFormat`)** and **browser locale (`navigator.language`)** to launch in the user's native language, with an instant live switcher in the top bar:
* 🇬🇧 **English** (Global Default)
* 🇹🇷 **Türkçe** (`Europe/Istanbul`)
* 🇩🇪 **Deutsch** (`Europe/Berlin`, `Vienna`, `Zurich`)
* 🇷🇺 **Русский** (`Europe/Moscow`, `Minsk`, `Almaty`)
* 🇪🇸 **Español** (`Europe/Madrid`, `America/Mexico_City`, `Buenos_Aires`)
* 🇫🇷 **Français** (`Europe/Paris`, `Brussels`)

---

### 6. Cryptographic Security & Ed25519 Pro Licensing
* **End-to-End SHA-256 Integrity:** Every transferred file is verified on disk with a cryptographic `SHA-256` hash.
* **Asymmetric Ed25519 Pro Verification:** Pro licenses (`PDPRO-CUSTOMER-...`) are signed offline using a 64-byte elliptic-curve `Ed25519` private key and verified mathematically inside the binary.

---

## 🛠️ Quick Start (30 Seconds)

1. Download **[PeerDrop-v4.2-Windows-x64.zip](./PeerDrop-v4.2-Windows-x64.zip)** and extract it to any folder.
2. Run **`peerdrop.exe`** *(passes built-in cryptographic self-audit, starts the HTTP/2 tunnel, and opens the desktop app window)*.
3. Click **`📱 Scan QR`** in the top bar:
   * **Same Wi-Fi Router:** Select **`📶 Local Wi-Fi (Max Speed)`** and scan with your phone.
   * **Anywhere (4G/5G / Remote):** Select **`🌍 Global (4G/5G / Anywhere)`** or click **`🔗 Invite Link`** to share via WhatsApp.
4. Tap the **📎 Paperclip** icon on your phone or drag files into the chat window to start streaming!

---

<div align="center">
  <b>Engineered by Barbaros Karagülmez (@barbarkaragul-oss)</b><br>
  <i>Low-Level Systems & High-Throughput P2P Network Architecture</i>
</div>