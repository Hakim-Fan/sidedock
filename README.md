# 🚀 SideDock - Official Support & Feedback Center

<p align="center">
  <strong>A Pure, Lightweight, and Instant-Access Slide-Over Sidebar Browser & Multitasking Workspace Utility Built Exclusively for macOS</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-macOS%2012.0%2B-green?logo=apple&logoColor=white" alt="Platform">
  <img src="https://img.shields.io/badge/Architecture-Apple%20Silicon%20%7C%20Intel-blue" alt="Architecture">
  <img src="https://img.shields.io/badge/Pricing-Fair%20%26%20Accessible-brightgreen" alt="Pricing">
  <img src="https://img.shields.io/badge/Data%20Privacy-Zero%20Telemetry-brightgreen" alt="Privacy">
  <img src="https://img.shields.io/badge/Technology-Native%20Swift%20%26%20AppKit-orange" alt="Tech">
  <img src="https://img.shields.io/badge/Community-GitHub%20Issues-blueviolet" alt="Community">
</p>

<p align="center">
  <a href="README.zh.md">简体中文</a> •
  <a href="README.md">English</a> •
  <a href="sidedock_privacy_policy.html">Privacy Policy (隐私政策)</a>
</p>

---

## 💡 Why SideDock? (Motivation)

**Slide Over on iPadOS** is one of the most delightful multitasking patterns ever designed—with a swift swipe from the edge, your notes, messengers, or reference materials glide into view and slip away just as effortlessly.

Yet on macOS, dependable slide-over utilities have been surprisingly scarce. Existing alternatives on the market either impose steep, recurring subscription models for users who simply want a reliable, lightweight slide-over companion, or run on resource-heavy cross-platform runtimes that eat up gigabytes of RAM and drain laptop batteries.

**Why shouldn't Mac users have a pure, native, battery-friendly sidebar without recurring subscription fatigue?**

That question sparked **SideDock**. Re-engineered from scratch using 100% native Swift and AppKit, powered directly by Apple's built-in WKWebView engine, and supercharged with **automated background tab sleeping** and **deep sleep resource freeing**, SideDock gives you an always-ready secondary screen that respects your machine and your wallet.

---

## 📌 Repository Notice

This repository serves as the official **Support Center, Issue Tracker, and Product Documentation** for **SideDock**.

If you encounter bugs, rendering issues, or have feature proposals, please feel free to open a [GitHub Issue](https://github.com/Hakim-Fan/slidepad-mac/issues). The **SideDock Team** actively reviews community feedback and iterates frequently!

---

## 📖 About SideDock

During everyday workflows—coding, writing technical documentation, attending virtual meetings, or multi-tasking—Mac users frequently jump back and forth between secondary web tools (such as instant messaging, online notes, AI utilities, translation tools, or documentation lookup) and their primary workspace. Cycling through multiple windows via `Command + Tab` disrupts focus, scatters attention, and clutters precious screen real estate.

**SideDock** silently docks on the right edge of your screen. Triggered by a global shortcut (default `Option + Space`), it glides out instantaneously. Check what you need, click back on your primary application, and it slides away automatically—leaving your workspace spotless.

---

## ⚖️ Why Choose SideDock? (Feature Comparison)

| Dimension | Legacy / Commercial Tools | **SideDock** |
| :--- | :--- | :--- |
| **Tech Stack** | Often bloated with cross-platform runtimes | **100% Native Swift + AppKit**, millisecond cold start |
| **Resource Efficiency** | Persistent tabs hog background CPU & RAM | **Smart Background Tab Sleep + Window Deep Sleep** |
| **Website Support** | Restricted catalogs or proprietary adapters | **Universal Omnibox**: load any URL or web app instantly |
| **Data Privacy** | Mandated cloud accounts, commercial tracking | **Zero Telemetry**, all data isolated in macOS sandbox |

---

## ✨ Key Highlights

### 🎯 Edge Slide-Over & Global Shortcut Summoning
- **One-Tap Global Toggle**: Default shortcut `Option + Space` (fully customizable via built-in key recorder in Preferences) to summon and tuck the sidebar instantaneously.
- **Fluid Spring Animation**: Powered by AppKit window-level physics tuning. Smooth edge alignment with flexible width adjustment.
- **Smart Auto-Dismissal**: Automatically and gracefully slides back into the screen edge when you click your main workspace, keeping your focus flow uninterrupted.
- **Multi-Monitor Awareness**: Intelligently tracks the display where your mouse cursor is currently active and slides out on that specific monitor.

### 📑 Independent Workspaces & Sidebar Tab Bar
- **Optimized Mobile & Compact Viewports**: Tailored viewport ratios and intelligent user-agent options provide clean, dense information layouts superior to bulky desktop web pages.
- **Rich Context Menu**: Convenient right-click actions for instant reloading, copying current URL, setting custom tab titles, or removing tabs.

### ⚡️ Smart Sleep Guard & Ultra-Low Resource Usage
- **Background Tab Sleep**: Inactive background tabs automatically freeze after a configurable interval, effectively preventing memory leaks and thermal throttling caused by heavy web apps.
- **Window Deep Sleep Mode**: When SideDock remains hidden for a specified period, all background web processes and heavy graphics allocations are released, reducing standby power draw to near zero.
- **Zero Electron Bloat**: Crafted in 100% native Swift with Apple's native WKWebView engine. Instant cold starts with minimal battery consumption.

### 🔒 Sandboxed Privacy & Zero Telemetry
- **Zero Telemetry Commitment**: Absolutely no proprietary relay servers, no behavioral tracking, and no third-party analytics SDKs. Your browsing data remains exclusively yours.
- **App Sandbox Protection**: All cookies, web caches, and local configurations are securely confined within the macOS application sandbox. One-click clearing of Web Cache & Cookies is always available in Preferences.

### 🌐 Dedicated Proxy Configuration
- **Dedicated Proxy Configuration**: Supports custom dedicated HTTP and SOCKS5 proxy server configurations for local development and specialized network environments.

---

## 📥 Download & Installation

- **Mac App Store**: Search for **`SideDock`** on the Mac App Store for one-click installation and seamless background updates.
- **System Requirements**: macOS 12.0 (Monterey) or later. Fully native across both Apple Silicon (M-series) and Intel architectures.

---

## 💡 Feedback & Support Guidelines

We deeply value your real-world feedback to help shape SideDock into the ultimate Mac utility:

### 1. Bug Reports
If you run into glitches, rendering issues, or application crashes, please open a [New Issue](https://github.com/Hakim-Fan/slidepad-mac/issues) and provide:
- Mac model and macOS version (e.g., MacBook Pro M3, macOS 15.0 / Mac mini Intel, macOS 13.5)
- App version (visible in Preferences)
- Steps to reproduce, accompanied by screenshots or console log excerpts

### 2. Feature Requests
Have an idea for gesture controls, edge snapping customization, tab grouping, or hotkey extensions? We would love to hear your thoughts on our GitHub Issues board!

---

## ❓ Frequently Asked Questions (FAQ)

<details>
<summary><strong>Q1: Does SideDock work seamlessly with multiple monitors and external displays?</strong></summary>
<p>Yes. SideDock dynamically tracks the screen edge where your mouse cursor is currently active and slides out accurately onto that display.</p>
</details>

<details>
<summary><strong>Q2: Will having a resident sidebar drain my battery or consume excessive RAM?</strong></summary>
<p>Not at all. SideDock completely eschews Electron in favor of native Swift and WKWebView. With built-in <strong>Background Tab Sleep</strong> and <strong>Window Deep Sleep</strong>, idle web processes are unloaded automatically when the dock is hidden, preserving both RAM and battery life.</p>
</details>

<details>
<summary><strong>Q3: Are my browsing history, passwords, or cookies uploaded to external servers?</strong></summary>
<p><strong>Absolutely not.</strong> SideDock is an offline-first client application. It does not operate any intermediate proxy or collection servers. Web requests travel directly from your device to the target website, with cookies and session storage isolated inside the macOS app sandbox.</p>
</details>

---

<p align="center">
  Crafted with care by the <strong>SideDock Team</strong> • Thank you for your support and feedback ❤️
</p>
