<div align="center">

# 🌐 Obsidian Polyglot Assistant

**A powerful language learning and translation companion for Obsidian**

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/Bif12/polyglot-assistant-plugin/releases)
[![Obsidian](https://img.shields.io/badge/Obsidian-Plugin-purple.svg)](https://obsidian.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Seamlessly integrates **Dictionary Lookup** for precise word definitions with **AI Translation** for contextual sentence translation, all within your Obsidian workspace.

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Settings](#%EF%B8%8F-settings) • [Support](#-support)

</div>

---

> **Note**: This is the **public release repository** for beta testing. It contains only release builds (no source code). If you'd like to contribute or view the source, please contact the author.

---

## ✨ Features

### 🔤 Dictionary Mode
- Instant word/phrase lookup with detailed definitions
- Multiple translations with synonyms
- Parts of speech categorization
- Plural forms and grammatical variations
- High-quality TTS audio pronunciation

### 🤖 AI Translator Mode
- Context-aware full sentence translation
- Real-time streaming translation (typing effect)
- Bidirectional translation (German ↔ Arabic, and more)
- Neural TTS audio for natural pronunciation
- Smart auto-detection of input language

### 📱 User Interface
- **Sidebar View**: Dedicated translation panel in the right sidebar with language direction indicator
- **Popup Tooltips**: Quick inline translations for selected text (up to 4 words)
- **Context Menu**: Right-click to translate selected text instantly
- **Editor Autocomplete**: Word suggestions while typing in your notes

### ⚙️ Smart Features
- **Automatic Language Detection**: Detects Arabic/Latin scripts and adjusts direction
- **Smart Mode Switching**: Automatically switches between Dictionary and AI based on text length
- **Auto-Translation Display Modes**: Choose between Sidebar, Popup, Both, or None
- **Language Pair Swapping**: One-click swap with reverse translation
- **Audio Caching**: Fast offline playback of previously fetched audio
- **Session Management**: Automatic session handling with retry logic

---

## 📦 Installation

### Manual Installation (Beta Testing)

1. Download the latest release from the [**Releases page**](https://github.com/Bif12/polyglot-assistant-plugin/releases)
2. Download all three files: `main.js`, `manifest.json`, `styles.css`
3. In your Obsidian vault, navigate to `.obsidian/plugins/`
4. Create a folder called `obsidian-polyglot`
5. Copy the three downloaded files into that folder:
   ```
   your-vault/
   └── .obsidian/
       └── plugins/
           └── obsidian-polyglot/
               ├── main.js
               ├── manifest.json
               └── styles.css
   ```
6. Restart Obsidian (or reload plugins)
7. Go to **Settings** → **Community Plugins** and enable **Polyglot Assistant**

### Using BRAT (Beta Reviewer's Auto-update Tester)

1. Install the [BRAT plugin](https://github.com/TfTHacker/obsidian42-brat) from Obsidian Community Plugins
2. Open BRAT settings
3. Click **"Add Beta Plugin"**
4. Enter this repository URL: `https://github.com/Bif12/polyglot-assistant-plugin`
5. Click **"Add Plugin"**
6. Enable **Polyglot Assistant** in Community Plugins

---

## 🚀 Usage

### Sidebar
1. Click the language icon in the ribbon (left sidebar)
2. Type a word or sentence in the input box
3. Press Enter or click the search button
4. Use the tabs to switch between Dictionary and AI modes

### Context Menu
1. Select any text in your note (1-4 words for popup, longer for sidebar)
2. Right-click to open the context menu
3. Choose:
   - **📖 Define**: Dictionary lookup for words
   - **🤖 AI Translate**: Full sentence translation
   - **🔊 Play Audio**: Hear pronunciation
   - **📋 Copy Translation**: Copy result to clipboard
   - **✍️ Insert Translation**: Insert translation inline

### Auto-Translation on Selection
1. Go to Settings → Polyglot → Auto Features
2. Choose **Auto-Translation Display**:
   - **Sidebar**: Automatically translate in sidebar when text is selected
   - **Popup**: Show inline popup tooltip for short phrases (≤4 words)
   - **Both**: Use both sidebar and popup
   - **None**: Disable auto-translation
3. Adjust **Popup Delay** (0-2000ms) for your preference

### Editor Autocomplete
1. Enable **Editor Autocomplete** in Settings → Auto Features
2. Start typing in your note (e.g., "restaur...")
3. Suggestions appear automatically after 2 characters
4. Use arrow keys to select, Enter to insert

### Commands (Ctrl/Cmd + P)
| Command | Description |
|---------|-------------|
| `Polyglot: Open Sidebar` | Open the translation sidebar |
| `Polyglot: Quick Translate` | Open modal for quick translation |
| `Polyglot: Define Selected Word` | Dictionary lookup for selection |
| `Polyglot: AI Translate Selection` | AI translate selected text |
| `Polyglot: Play Audio` | Play pronunciation for selected text |
| `Polyglot: Swap Languages` | Switch source ↔ target languages |
| `Polyglot: Clear Audio Cache` | Free up storage space |
| `Polyglot: Refresh Session` | Reconnect to translation service |

---

## ⚙️ Settings

### General
- **Source Language**: Choose your source language (de, en, fr, ar)
- **Target Language**: Choose your target language (ar, de, en)
- **Default View**: Sidebar or Modal for new translations
- **Auto-Detect**: Automatically detect and swap language direction based on input

### AI & Performance
- **Smart Switching**: Auto-switch between Dictionary and AI modes based on content
- **AI Trigger Threshold**: Number of words to trigger AI mode (default: 3)
- **Streaming**: Show translation text as it generates (live typing effect)

### Dictionary Filters
- **Show Synonyms**: Display alternative translations
- **Show Plurals**: Show plural forms when available
- **Show Definitions**: Display detailed word definitions
- **Strict Mode**: Exact matches only (experimental)

### Auto Features
- **Auto-Translation Display**: Choose where to show translations on text selection
- **Popup Delay**: Milliseconds before auto-translation triggers (0-2000ms)
- **Sidebar Autocomplete**: Show suggestions in sidebar search box
- **Editor Autocomplete**: Show word suggestions while typing in notes

---

## 🌍 Supported Languages

| Language Pair | Support Level |
|---------------|---------------|
| 🇩🇪 German ↔ 🇸🇦 Arabic | ✅ Full bidirectional |
| 🇬🇧 English    |  🔜 Coming soon |
---

## 🔧 Troubleshooting

### Translation Not Working
1. Check Settings → System → Session Status
2. Click "Refresh Session" if inactive
3. Verify internet connection

### Audio Not Playing
1. Clear audio cache (Settings → System)
2. Check browser audio permissions
3. Refresh session

### Autocomplete Not Appearing
1. Enable "Editor Autocomplete" in Settings → Auto Features
2. Type at least 2 characters
3. Ensure you're typing in a markdown editor

---

## 📞 Support

- 🐛 **Bug Reports**: [GitHub Issues](https://github.com/Bif12/polyglot-assistant-plugin/issues)
- 💡 **Feature Requests**: [GitHub Issues](https://github.com/Bif12/polyglot-assistant-plugin/issues)
- 📧 **Contact**: khalid.bifounra.98@edu.uiz.ac.ma

---

## 📄 License

This project is licensed under the **MIT License**.

---

<div align="center">

**If you find this plugin useful, please consider giving it a ⭐!**

Made with ❤️ for the Obsidian community by [Bif12](https://github.com/Bif12)

</div>
