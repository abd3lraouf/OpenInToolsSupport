# OpenInTools Changelog

All notable changes to this project will be documented in this file.

## [2.3.0] - 2026-01-05

### Added
- **Expanded Platform Support** - Now supports IntelliJ IDEA 2024.1 and later (previously 2025.2+)
  - Compatible with all JetBrains IDEs from 2024.1 onwards
  - Includes Android Studio 2024.1+

### Improved
- **Xcode Dropdown Behavior** - Play button now properly switches between selection and direct-open modes
  - When play button is visible: click to select, play button to open
  - When play button is hidden: click to open immediately
  - Rescan and Configure always work immediately

## [2.2.4] - 2026-01-05

### Fixed
- **Xcode Project Scanning** - Fixed "Scanning for projects..." that would never complete on some Android Studio versions

## [2.2.3] - 2026-01-01

### Improved
- **Settings UI Overhaul** - Complete redesign of the Open In Tools settings panel
  - Table-based tool configuration with inline editing
  - Add/remove tools with smart detection
  - "Detect All" button to auto-discover installed tools
  - Drag-and-drop ordering for toolbar and context menu
- **Attribution Panel** - Updated developer attribution

### Fixed
- **Play Button Default** - Xcode play button in toolbar now disabled by default
- **UI Polish** - Various spacing and alignment improvements in settings

## [2.2.2] - 2026-01-01

### Fixed
- **Incorrect Settings Navigation** - Fixed error messages pointing to non-existent settings page
- **Robust Tool Detection** - Improved detection accuracy across all platforms

### Improved
- **Windows Detection** - Better support for various installation locations and package managers
- **Linux Detection** - Full XDG compliance, Flatpak and Snap support

## [2.2.1] - 2026-01-01

### Fixed
- **False Detection of Uninstalled Apps** - Tools now correctly show as "not detected" when the app is uninstalled
- **Path Display** - Clean app bundle paths shown in settings instead of internal executables

## [2.2.0] - 2026-01-01

### Added
- **Smart App Detection** - Intelligent platform-aware application discovery
  - **macOS**: Uses Spotlight for instant, accurate detection
  - **Windows**: Searches registry and common installation paths
  - **Linux**: Searches desktop files and system paths
- **Path Normalization** - Automatically cleans up internal app paths for better display

### Improved
- **Detection Accuracy** - More reliable tool detection across all platforms

## [2.1.2] - 2026-01-01

### Improved
- **Native Xcode Dropdown** - Uses native JetBrains popup for better look and feel
- **Dynamic Updates** - Xcode dropdown refreshes in real-time when project scan completes
- **Searchable Settings** - Find settings via IDE's Settings search

### Fixed
- **Threading Stability** - Improved background task handling
- **Memory Usage** - Fixed resource leaks in popup components

## [2.1.1] - 2026-01-01

### Fixed
- **Compatibility** - Fixed error when opening Xcode dropdown in IntelliJ 2025.3+
- **Plugin Icon** - Fixed icon display in IDE plugin browser

## [2.1.0] - 2026-01-01

### Added
- **Xcode Toolbar Dropdown** - Android Studio-style configuration selector with integrated chevron
- **Play Button Toggle** - Option to show/hide play button in toolbar (Settings > Xcode > Toolbar Behavior)
- **Direct Open Mode** - When play button is hidden, clicking configurations opens them immediately
- **Intelligent Plist Opening** - Info.plist files open within their containing workspace/project context
- **Project Discovery** - Background scanning for Xcode workspaces, projects, and Info.plist files

### Improved
- **Xcode Integration** - Better file reveal in Xcode
- **Settings Persistence** - Xcode toolbar settings persist across sessions

### Fixed
- **Toolbar Appearance** - Correct button margins matching Android Studio's style
- **Popup Selection** - Mouse hover correctly highlights items

## [2.0.0] - 2025-12-31

### Added
- **Expanded Tool Support** - Added Fleet, Zed, Sublime Text, and Windsurf editors
- **Quick Switcher** - Press `Cmd+Shift+O` / `Ctrl+Shift+O` to quickly switch between tools
- **Context Menu Integration** - Right-click on files, folders, or tabs to open in external tools
- **Open at Cursor Position** - Opens files at exact line and column in supporting editors
- **Reveal in Xcode** - Navigate to specific files in Xcode's Project Navigator (`Cmd+Shift+X`)
- **Separate Ordering** - Configure toolbar and context menu order independently
- **Tool Aliases** - Search tools by aliases in quick switcher
- **Recent Tools Tracking** - Quick switcher shows recently used tools first

### Improved
- **Dynamic Toolbar** - Toolbar dynamically shows enabled tools in configured order
- **Settings UI** - Redesigned settings with drag-and-drop ordering

## [1.0.1] - 2025-04-29

### Improved
- Enhanced theme integration
- Better settings UI clarity
- Improved notification messages

## [1.0.0] - 2025-04-29

### Added
- Initial implementation of the OpenInTools plugin
- VS Code support for opening projects
- Cursor support for opening projects
- Xcode support for opening projects/workspaces (macOS only)
- Settings page to configure tool paths
- Auto-detection of tools on various platforms
- Cross-platform support (Windows, macOS, Linux)
