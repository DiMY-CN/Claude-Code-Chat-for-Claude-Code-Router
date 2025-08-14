# Settings Interface Test Plan

## Overview
Added a settings interface to the Claude Code Chat webview that allows users to configure WSL settings.

## Changes Made

### 1. UI Changes (ui.ts)
- Added a settings button (⚙️) in the header that's always visible
- Created a settings modal with WSL configuration options:
  - Enable WSL Integration checkbox
  - WSL Distribution input field
  - Node.js Path in WSL input field
  - Claude Path in WSL input field
- Added JavaScript functions:
  - `toggleSettings()` - Shows/hides the settings modal
  - `hideSettingsModal()` - Hides the settings modal
  - `updateSettings()` - Sends settings changes to VS Code
  - Event listeners for modal interaction

### 2. Extension Changes (extension.ts)
- Added message handlers:
  - `getSettings` - Retrieves current settings from VS Code configuration
  - `updateSettings` - Updates VS Code configuration with new settings
- Added methods:
  - `_sendCurrentSettings()` - Sends current settings to webview
  - `_updateSettings()` - Updates VS Code configuration

### 3. Configuration (package.json)
- Already has WSL configuration properties defined:
  - `claudeCodeChat.wsl.enabled`
  - `claudeCodeChat.wsl.distro`
  - `claudeCodeChat.wsl.nodePath`
  - `claudeCodeChat.wsl.claudePath`

## Testing Steps

1. Open VS Code with the extension
2. Open Claude Code Chat (Ctrl+Shift+C)
3. Click the settings button (⚙️) in the header
4. Verify the settings modal appears
5. Check that current WSL settings are loaded
6. Toggle "Enable WSL Integration" and verify:
   - WSL options show/hide accordingly
   - Settings are saved when changed
7. Modify WSL settings and verify they persist
8. Close and reopen the settings to confirm values are saved

## Features

- Settings button is always visible in the header
- Modal design matches the existing tools modal
- Real-time show/hide of WSL options based on enabled state
- Settings persist across sessions
- Success/error notifications when saving settings