# SoundPeek

![Build](https://github.com/Jaroslav01/SoundPeek/workflows/Build/badge.svg)
[![Version](https://img.shields.io/jetbrains/plugin/v/MARKETPLACE_ID.svg)](https://plugins.jetbrains.com/plugin/MARKETPLACE_ID)
[![Downloads](https://img.shields.io/jetbrains/plugin/d/MARKETPLACE_ID.svg)](https://plugins.jetbrains.com/plugin/MARKETPLACE_ID)

## Template ToDo list
- [x] Create a new [IntelliJ Platform Plugin Template][template] project.
- [ ] Get familiar with the [template documentation][template].
- [ ] Adjust the [pluginGroup](./gradle.properties) and [pluginName](./gradle.properties), as well as the [id](./src/main/resources/META-INF/plugin.xml) and [sources package](./src/main/kotlin).
- [ ] Adjust the plugin description in `README` (see [Tips][docs:plugin-description])
- [ ] Review the [Legal Agreements](https://plugins.jetbrains.com/docs/marketplace/legal-agreements.html?from=IJPluginTemplate).
- [ ] [Publish a plugin manually](https://plugins.jetbrains.com/docs/intellij/publishing-plugin.html?from=IJPluginTemplate) for the first time.
- [ ] Set the `MARKETPLACE_ID` in the above README badges. You can obtain it once the plugin is published to JetBrains Marketplace.
- [ ] Set the [Plugin Signing](https://plugins.jetbrains.com/docs/intellij/plugin-signing.html?from=IJPluginTemplate) related [secrets](https://github.com/JetBrains/intellij-platform-plugin-template#environment-variables).
- [ ] Set the [Deployment Token](https://plugins.jetbrains.com/docs/marketplace/plugin-upload.html?from=IJPluginTemplate).
- [ ] Click the <kbd>Watch</kbd> button on the top of the [IntelliJ Platform Plugin Template][template] to be notified about releases containing new features and fixes.

<!-- Plugin description -->
This Fancy IntelliJ Platform Plugin is going to be your implementation of the brilliant ideas that you have.

This specific section is a source for the [plugin.xml](/src/main/resources/META-INF/plugin.xml) file which will be extracted by the [Gradle](/build.gradle.kts) during the build process.

To keep everything working, do not remove `<!-- ... -->` sections. 
<!-- Plugin description end -->

## Installation

- Using the IDE built-in plugin system:
  
  <kbd>Settings/Preferences</kbd> > <kbd>Plugins</kbd> > <kbd>Marketplace</kbd> > <kbd>Search for "SoundPeek"</kbd> >
  <kbd>Install</kbd>
  
- Using JetBrains Marketplace:

  Go to [JetBrains Marketplace](https://plugins.jetbrains.com/plugin/MARKETPLACE_ID) and install it by clicking the <kbd>Install to ...</kbd> button in case your IDE is running.

  You can also download the [latest release](https://plugins.jetbrains.com/plugin/MARKETPLACE_ID/versions) from JetBrains Marketplace and install it manually using
  <kbd>Settings/Preferences</kbd> > <kbd>Plugins</kbd> > <kbd>⚙️</kbd> > <kbd>Install plugin from disk...</kbd>

- Manually:

  Download the [latest release](https://github.com/Jaroslav01/SoundPeek/releases/latest) and install it manually using
  <kbd>Settings/Preferences</kbd> > <kbd>Plugins</kbd> > <kbd>⚙️</kbd> > <kbd>Install plugin from disk...</kbd>


---
Plugin based on the [IntelliJ Platform Plugin Template][template].

[template]: https://github.com/JetBrains/intellij-platform-plugin-template
[docs:plugin-description]: https://plugins.jetbrains.com/docs/intellij/plugin-user-experience.html#plugin-description-and-presentation


# 🎧 SoundPeek *(early concept stage)*

> ⚠️ This project is currently in the **idea/prototype stage**.  
> Contributions, feedback, and collaboration are welcome!

**SoundPeek** is a JetBrains Rider plugin that allows you to **preview audio data during debugging**.

When debugging, simply **hover over or select a variable** containing audio data — such as a Base64-encoded string or raw byte array — and play the sound with a single click.  
It supports various audio formats via `ffplay` (from FFmpeg), making it ideal for developers working with voice, media, or binary protocols.

---

## 🚀 Features

- 🔍 Detects audio data in variables (e.g. Base64 strings, byte arrays)
- ▶️ Plays audio on demand using `ffplay` or a configurable external player
- ⚙️ Supports multiple formats: MP3, WAV, OGG, FLAC, etc.
- 🛠 Works directly from the debugger with minimal setup
- 🧪 Useful for audio processing, speech synthesis, binary debugging, and more

---

## 📦 Requirements

- JetBrains Rider (2023.1+ recommended)
- [FFmpeg](https://ffmpeg.org/download.html) with `ffplay` available in PATH

---

## 🛠 Installation

### Option 1: From Disk

1. Clone or download this repository.
2. Run `./gradlew buildPlugin`.
3. Go to `Settings > Plugins > Install Plugin from Disk` in Rider.
4. Choose the generated `.zip` file from `build/distributions`.

### Option 2: From JetBrains Marketplace *(planned)*

---

## 🎮 How to Use

1. Start debugging in Rider.
2. Hover over or select a variable containing Base64-encoded audio or binary data.
3. Right-click and select `Play with SoundPeek`, or use the toolbar action.
4. Listen to the sound — no need to export or manually decode!

---

## 📷 Screenshots *(coming soon)*

---

## 🔧 Configuration (optional)

You can configure the path to your preferred audio player (e.g., `ffplay`, `afplay`, `vlc`, etc.) in the plugin settings.

---

## 🧑‍💻 Why SoundPeek?

Working with audio or binary protocols during debugging often involves manual decoding and saving files — SoundPeek eliminates that hassle. Whether you're working on:

- 🎙 Speech-to-text or TTS engines  
- 🧬 Binary protocols or custom encodings  
- 🔊 Game audio or music apps  
- 🎥 Media streaming/debugging tools  

...SoundPeek helps you *hear what's going on*.

---

## 🛡 License

MIT License

---

## 🤝 Contributing

Pull requests, feedback, and suggestions are welcome!  
See [CONTRIBUTING.md](CONTRIBUTING.md) *(coming soon)*.

---

## 📫 Contact

Feel free to open an issue or contact the author via GitHub.

---

