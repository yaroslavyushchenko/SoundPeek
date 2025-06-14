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

