# OpenInTools Changelog

All notable changes to this project will be documented in this file.

## [2.1.0] - 2026-01-01

### Added
- **Xcode Toolbar Dropdown** - Android Studio-style configuration selector with integrated chevron
- **Play Button Toggle** - Option to show/hide play button in toolbar (Settings > Xcode > Toolbar Behavior)
- **Direct Open Mode** - When play button is hidden, clicking configurations opens them immediately
- **Intelligent Plist Opening** - Info.plist files open within their containing workspace/project context
- **Project Discovery** - Background scanning for Xcode workspaces, projects, and Info.plist files
- **Release Script** - Local validation script matching CI workflow

### Changed
- **Improved Xcode Integration** - Uses AppleScript for better file reveal in Xcode
- **Settings Persistence** - Xcode toolbar settings now persist across sessions
- **Better UX** - No checkmarks in direct open mode (selection vs direct)

### Fixed
- **Toolbar Button Padding** - Correct margins matching Android Studio's run configuration selector
- **Popup Selection** - Mouse hover correctly highlights items in dropdown

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

### Changed
- **Dynamic Toolbar** - Toolbar now dynamically shows enabled tools in configured order
- **Improved Settings UI** - Redesigned settings with drag-and-drop ordering
- **Better Architecture** - Refactored to follow SOLID principles

## [1.0.1] - 2025-04-29

### Changed
- Enhanced Xcode action component for improved theme integration
- Refactored settings UI for better clarity
- Updated notification messages

## [1.0.0] - 2025-04-29

### Added
- Initial implementation of the OpenInTools plugin
- VS Code support for opening projects
- Cursor support for opening projects
- Xcode support for opening projects/workspaces (macOS only)
- Settings page to configure tool paths
- Auto-detection of tools on various platforms
- Cross-platform support (Windows, macOS, Linux)
