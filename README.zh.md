# 🚀 SideDock - 官方支持与用户反馈中心

<p align="center">
  <strong>一款专为 macOS 打造的高效、轻盈、即开即用的边缘抽屉式侧边栏浏览器与多任务工作区辅助工具</strong>
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
  <a href="sidedock_privacy_policy.html">隐私政策 (Privacy Policy)</a>
</p>

---

## 💡 诞生初衷 (Why SideDock)

iPadOS 上的 **Slide Over（侧拉浮窗）** 是一种极为优雅的多任务交互形态——在主屏幕专注工作的同时，轻轻一滑就能随手查词典、回复消息或记录灵感，用完即收。

但在 macOS 上，长久以来缺乏一款趁手的边缘抽屉工具。市面上同类产品要么推行昂贵的持续订阅制模式，让许多只是想要一个稳定、纯粹的常驻侧边小窗的用户望而却步；要么基于臃肿的跨平台框架构建，常驻后台动辄吞噬数 GB 内存和大量电量。

**为什么不能有一款原生、纯粹、无高昂订阅负担，且对系统资源极其克制的工具？**

于是，**SideDock** 诞生了。我们使用纯原生 Swift + AppKit 重构了边缘滑动窗口，依托系统底层 WKWebView 提供极速渲染，并创新加入了独创的**后台标签自动休眠**与**窗口深度睡眠机制**。让每一位 Mac 用户都能毫无负担地拥有一个如丝般顺滑的“常驻第二屏幕”。

---

## 📌 仓库说明 (Repository Notice)

本仓库为 **SideDock** 的官方用户反馈中心、问题跟进平台与文档主页。

如果您在使用过程中遇到任何问题、渲染异常，或有好的产品建议、功能需求，欢迎随时在此提交 [Issue](https://github.com/Hakim-Fan/slidepad-mac/issues)。**SideDock团队** 会定期查看并持续跟进处理！

---

## 📖 关于 SideDock (About)

在日常使用 Mac 进行编程开发、技术写作、音视频会议或综合办公时，我们总需要在主工作区与各类辅助网页之间频繁周旋（例如：即时通讯、在线笔记、AI 工具、翻译词典、参考手册等）。频繁使用 `Command + Tab` 切换不仅容易打乱思维心流，还会让桌面堆满层层叠叠的杂乱窗口。

**SideDock** 始终静默潜伏在屏幕边缘。通过自定义全局快捷键（默认 `Option + Space`），只需轻轻一按，侧边栏即刻滑出，查完随手点击主屏幕即自动缩回，彻底释放您的桌面空间。

---

## ⚖️ 为什么选择 SideDock？(Feature Comparison)

| 核心特性 | 传统常驻侧边栏 / 商业竞品 | **SideDock** |
| :--- | :--- | :--- |
| **底层技术架构** | 部分采用跨平台框架，体积庞大耗电 | **100% 纯原生 Swift + AppKit**，毫秒级冷启 |
| **内存与能耗控制** | 多标签常驻后台，易发热导致内存暴涨 | **内置后台标签自动休眠 + 窗口深睡释放机制** |
| **自由添加网址** | 部分工具限制站点，必须等待官方适配 | **通用 Omnibox**，输入任意网址/搜索引擎即用 |
| **数据与隐私安全** | 强制注册账号，可能集成商业追踪埋点 | **零遥测（Zero Telemetry）**，本地沙盒隔离存储 |

---

## ✨ 核心功能亮点 (Highlights)

### 🎯 边缘悬浮触达与全局快捷唤醒
- **一键全局呼出**：默认快捷键 `Option + Space`（支持在设置中自定义录制任意快捷键），随时召唤与收起。
- **物理弹性顺滑手势**：精心调优的 Spring 弹簧动效，精准吸附屏幕右侧边缘，支持鼠标拖拽自适应调节面板宽度。
- **智能失焦自动隐藏**：在侧边栏查完信息后，点击主工作区任意位置，侧边栏立即优雅滑回边缘，完全不干扰主任务。
- **多显示器自适应**：智能感知当前鼠标光标所在的屏幕边缘，在正在工作的显示器上即时呼出。

### 📑 独立多工作区与侧边标签栏
- **移动端与桌面端智能自适应**：针对窄屏小窗特别调优视口与排版，获得比传统桌面网页更清爽轻量的信息密度。
- **丰富的标签管理**：右键菜单支持快速重新加载、复制当前 URL、自定义应用标题、替换站点图标与删除。

### ⚡️ 独创智能内存休眠守护（低能耗长驻）
- **后台标签自动休眠（Background Tab Sleep）**：长时间未被前台点击的非活跃后台标签，系统自动将其挂起冻结，大幅减轻 CPU 负荷与内存占用。
- **窗口深睡模式（Window Deep Sleep）**：当 SideDock 隐藏一段预设时长后，自动释放后台网页图形上下文与非必要进程资源，常驻耗电趋近于零。
- **拒绝 Electron 臃肿**：采用原生系统内核，彻底告别数百兆的打包体积和动辄发热卡顿的困扰。

### 🔒 纯本地运行与沙盒隐私安全
- **零遥测与零追踪（Zero Telemetry）**：不设任何自建中转服务器，无任何第三方埋点、行为追踪或画像 SDK。
- **沙盒安全隔离**：网页 Cookie、缓存与工作区配置文件严格存储于 macOS 本地沙盒，支持在偏好设置中一键彻底清理 Web 缓存与 Cookie。

### 🌐 网络与专用代理设置
- **网络与专用代理设置**：支持单独配置专有 HTTP / SOCKS5 代理端口，满足开发调试与跨网络访问需求。

---

## 📥 获取与安装 (Download & Install)

- **Mac App Store**：在 Mac App Store 搜索 **`SideDock`** 即可一键下载安装与自动静默更新。
- **系统要求**：macOS 12.0 (Monterey) 及更高版本，原生支持 Apple Silicon M系列与 Intel 架构机型。

---

## 💡 如何提交反馈与建议 (Feedback & Support)

我们非常重视每一位开发者的真实使用体验，欢迎通过以下方式参与产品改进：

### 1. 提交 Bug 报告 (Bug Report)
如果您在使用中遇到异常或崩溃，请前往 [New Issue](https://github.com/Hakim-Fan/slidepad-mac/issues) 并提供以下信息：
- 设备机型与系统版本（例如：MacBook Pro M2, macOS 14.5 / iMac Intel, macOS 13.6）
- 应用版本号（可在偏好设置中查看）
- 具体的复现步骤、问题截图或控制台异常输出

### 2. 提出新功能需求 (Feature Request)
如果您有关于侧边栏交互、手势操作、工作区分类、快捷键扩展等任何灵感与建议，欢迎在 Issues 中开帖畅所欲言！

---

## ❓ 常见问题 (FAQ)

<details>
<summary><strong>Q1: 可以在不同屏幕或者多个外接显示器上使用 SideDock 吗？</strong></summary>
<p>可以。SideDock 会智能识别当前鼠标活跃聚焦的显示器屏幕边缘，随时在您当前工作的那块屏幕上精准滑出。</p>
</details>

<details>
<summary><strong>Q2: 侧边栏常驻会不会消耗大量 Mac 内存和电量？</strong></summary>
<p>绝对不会。SideDock 放弃了体积庞大的 Electron 方案，转而采用纯原生 Swift 与 macOS 深度集成的 WKWebView。不仅如此，内置的<strong>后台标签自动休眠</strong>和<strong>窗口深睡模式</strong>会在窗口收起后自动释放网页进程，即便长期待机也几乎不耗电。</p>
</details>

<details>
<summary><strong>Q3: 我的网页浏览历史、登录密码和 Cookies 会被上传吗？</strong></summary>
<p><strong>绝对不会。</strong> SideDock 是一款纯客户端应用，不设有任何中转或采集服务器。所有网页的通信均由您的 Mac 直连目标网站，生成的 Cookies 和 LocalStorage 全部受 macOS 官方应用沙盒隔离保护，开发者无法亦无意愿获取您的任何数据。</p>
</details>

---

<p align="center">
  由 <strong>SideDock团队</strong> 倾心打造 • 期待您的宝贵反馈与支持 ❤️
</p>
