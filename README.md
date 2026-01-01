<p align="center">
  <img src="art/OpenInTools.png" width="200" alt="OpenInTools Logo"/>
</p>

<h1 align="center">OpenInTools Support</h1>

<p align="center">
  <b>Official support repository for the OpenInTools IntelliJ plugin</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Version-2.1.1-success.svg" alt="Version 2.1.1">
  <a href="https://plugins.jetbrains.com/plugin/27235-open-in-tools"><img src="https://img.shields.io/jetbrains/plugin/d/27235-open-in-tools.svg" alt="Downloads"></a>
  <img src="https://img.shields.io/badge/IntelliJ-2025.2+-07C3F2.svg" alt="IntelliJ 2025.2+">
  <img src="https://img.shields.io/badge/macOS%20|%20Windows%20|%20Linux-lightgrey.svg" alt="Platforms">
</p>

<p align="center">
  <a href="#-about">About</a> •
  <a href="#-features">Features</a> •
  <a href="#-supported-tools">Tools</a> •
  <a href="#-xcode-integration">Xcode</a> •
  <a href="#-reporting-issues">Issues</a> •
  <a href="#-faq">FAQ</a>
</p>

---

## 📖 About

This is the official support channel for **OpenInTools** — the plugin that bridges your JetBrains IDE with your favorite external editors.

**One click to VS Code. One click to Cursor. One click to Xcode. No friction, just flow.**

> The main plugin repository is private. All support, issues, and feature requests are handled here.

<p align="center">
  <a href="https://plugins.jetbrains.com/plugin/27235-open-in-tools">
    <img src="https://img.shields.io/badge/Install%20from-JetBrains%20Marketplace-07C3F2?style=for-the-badge&logo=jetbrains" alt="Install from JetBrains Marketplace"/>
  </a>
</p>

## ✨ Features

### Toolbar Integration

One-click access to all your favorite editors directly from the toolbar.

<p align="center">
  <img src="art/screenshots/toolbar.png" width="700" alt="Toolbar Integration"/>
</p>

### Context Menu

Right-click any file, folder, or editor tab to open in external tools.

<p align="center">
  <img src="art/screenshots/context-menu.png" width="500" alt="Context Menu"/>
</p>

### Quick Switcher

Press `Cmd+Shift+O` / `Ctrl+Shift+O` for fuzzy search with aliases and recent tools first.

<p align="center">
  <img src="art/screenshots/quick-actions.png" width="500" alt="Quick Switcher"/>
</p>

### Feature Overview

| Feature | Description |
|---------|-------------|
| **One-Click Launch** | Toolbar buttons open your project instantly |
| **Open at Cursor** | Jumps to exact line:column in the target editor |
| **Quick Switcher** | `Cmd+Shift+O` — fuzzy search, aliases, recent tools first |
| **Context Menus** | Right-click any file, folder, or tab |
| **Drag & Drop Order** | Customize toolbar and menu order separately |
| **Auto-Detection** | Finds installed tools automatically |

## 🛠 Supported Tools

| Editor | Platforms | Open at Line | Quick Aliases |
|--------|-----------|:------------:|---------------|
| **VS Code** | All | ✅ | `vsc`, `code` |
| **Cursor** | All | ✅ | `cur`, `ai` |
| **Fleet** | All | ✅ | `flt`, `jb` |
| **Zed** | macOS, Linux | ✅ | `z` |
| **Sublime Text** | All | ✅ | `subl`, `st` |
| **Windsurf** | All | ✅ | `ws`, `surf` |
| **Xcode** | macOS | — | `xc`, `ios` |

## 🍎 Xcode Integration

**Native-feeling Xcode integration** for Kotlin Multiplatform and iOS developers.

### Android Studio-Style Dropdown

The Xcode toolbar button works just like Android Studio's run configuration selector:
- **Dropdown menu** with all discovered workspaces and projects
- **Integrated chevron** — click anywhere on the button
- **Play button** to launch the selected configuration

### Two Modes

| Mode | Play Button | Click Behavior |
|------|:-----------:|----------------|
| **Selection Mode** | ✅ Visible | Selects config, click play to launch |
| **Direct Mode** | ❌ Hidden | Opens immediately on click |

### Smart Project Discovery

- **Workspaces** (`.xcworkspace`) — CocoaPods, SPM, multi-target projects
- **Projects** (`.xcodeproj`) — Standalone Xcode projects
- **Info.plist** — Quick access to app configuration files
- **Intelligent Opening** — Plist files open within their workspace context

### Reveal in Xcode

Press `Cmd+Shift+X` to reveal the current file in Xcode's Project Navigator.

## ⚙️ Configuration

**Settings → Tools → Open In Tools**

### Main Settings

Configure which tools appear in toolbar and context menus, drag to reorder, and set custom paths.

<p align="center">
  <img src="art/screenshots/settings-main.png" width="700" alt="Main Settings"/>
</p>

### Xcode Settings (macOS)

Configure Xcode-specific options: workspace/project scanning, play button visibility, and more.

<p align="center">
  <img src="art/screenshots/settings-xcode.png" width="700" alt="Xcode Settings"/>
</p>

## 🐛 Reporting Issues

Found a bug? [Create a new issue](https://github.com/abd3lraouf/OpenInToolsSupport/issues/new) with:

1. **Description** — Clear description of the issue
2. **Steps to Reproduce** — How to trigger the problem
3. **Expected vs Actual** — What should happen vs what happens
4. **Environment** — OS, IDE version, plugin version
5. **Screenshots** — If applicable

## 💡 Feature Requests

Have an idea? [Submit a feature request](https://github.com/abd3lraouf/OpenInToolsSupport/issues/new):

- Use title format: `[Feature] Your Idea`
- Describe the use case and benefits
- Include mockups if possible

## ❓ FAQ

<details>
<summary><b>Which IDEs are supported?</b></summary>

All JetBrains IDEs: IntelliJ IDEA, Android Studio, WebStorm, PyCharm, GoLand, Rider, etc.
</details>

<details>
<summary><b>Is Xcode integration available on Windows/Linux?</b></summary>

No, Xcode is macOS-only. The Xcode features only appear on macOS.
</details>

<details>
<summary><b>How does tool detection work?</b></summary>

The plugin searches common installation paths. You can also set custom paths in Settings → Tools → Open In Tools.
</details>

<details>
<summary><b>Can I open specific files instead of the whole project?</b></summary>

Yes! Use the context menu on any file, folder, or editor tab. Files open at the exact cursor position in supporting editors.
</details>

<details>
<summary><b>How do I change the toolbar order?</b></summary>

Settings → Tools → Open In Tools. Drag and drop to reorder. Toolbar and context menu have separate ordering.
</details>

## 📝 Release Notes

See [CHANGELOG.md](CHANGELOG.md) for version history.

### What's New in 2.1.1

- **Fixed:** DataContext error when opening Xcode dropdown in IntelliJ 2025.3+
- **Fixed:** Plugin icon now displays correctly in IDE plugin browser

### What's New in 2.1.0

- **Xcode Toolbar Dropdown** — Android Studio-style configuration selector
- **Play Button Toggle** — Choose between selection mode and direct open mode
- **Intelligent Plist Opening** — Opens within workspace/project context
- **Background Project Discovery** — Async scanning with caching

## 📄 License

**Proprietary Software** — © 2025-2026 Abdelraouf Sabri. All Rights Reserved.

This software is not open source. See [LICENSE](LICENSE) for terms.

---

<p align="center">
  <b>Built for developers who use multiple tools.</b><br>
  <sub>© 2025-2026 <a href="https://github.com/abd3lraouf">Abdelraouf Sabri</a> — All Rights Reserved</sub>
</p>
