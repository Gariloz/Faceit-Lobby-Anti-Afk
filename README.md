# Faceit Lobby Anti Afk

**Faceit Lobby Anti Afk** is a userscript for Tampermonkey/Greasemonkey that automatically clicks the "Keep open" button in FACEIT modal windows, preventing automatic lobby closure due to inactivity.

## Main Features

* Automatically clicks "Keep open" button when modal appears
* Universal button detection - works regardless of FACEIT selector changes
* Multi-language support (English and Russian interfaces)
* Dual detection system (MutationObserver + interval fallback)
* Works on all FACEIT pages (*.faceit.com)
* Silent operation - no console logging
* Reliable modal window detection
* Protection against multiple clicks
* Toggle button for easy enable/disable functionality
* State persistence across browser sessions and page reloads

## Installation

### Option 1: Without Extension (Quick Start)

1. Open any FACEIT page
2. Open browser console (`F12` or `Ctrl+Shift+J` / `Cmd+Option+J` on Mac)
3. Open `Faceit-Lobby-Anti-Afk.user.js` file and copy all code
4. **IMPORTANT**: Delete the first 9 lines (metadata starting with `// ==UserScript==` and ending with `// ==/UserScript==`)
5. Paste the remaining code (starting from line 11 with `(function() {`) into console and press `Enter`
6. Click the green "Включить анти-афк" button to activate

⚠️ **Note**: Script stops after page reload. You'll need to run it again.

### Option 2: With Tampermonkey/Greasemonkey (Recommended)

1. Install Tampermonkey or Greasemonkey browser extension
2. Download the `Faceit-Lobby-Anti-Afk.user.js` file
3. Click on the userscript file to install it in Tampermonkey
4. Navigate to any FACEIT page
5. Script automatically activates (enabled by default)

✅ **Advantage**: Script works automatically on every page load.

## Usage

* Script is enabled by default when installed
* Click the green "Включить анти-афк" button to activate the script
* Click the red "Отключить анти-афк" button to deactivate
* Button changes color to indicate status:
  - **Green**: Script disabled
  - **Red**: Script active and monitoring
* Click the eye icon (👁️) on the button to hide it - a small eye icon will appear in its place
* Click the small eye icon to show the button again
* Script remembers state across page reloads
* Automatically detects and clicks "Keep open" buttons when modal appears
* Works with party/lobby inactivity modals

## Changes in Version

* **Universal selector support** - Works with old and new FACEIT modal structures
* **Multi-language button detection** - Supports English and Russian text
* **Dual detection system** - MutationObserver + interval for maximum reliability
* **Silent operation** - No console output for clean operation
* **Reliable modal detection** - Multiple selector fallbacks for maximum compatibility
* **Toggle button** - Easy enable/disable functionality
* **State persistence** - Remembers enabled/disabled state across sessions using localStorage
* **Default enabled** - Script is active by default when installed

## GitHub

https://github.com/Gariloz/Faceit-Lobby-Anti-Afk

---

**Author:** Gariloz