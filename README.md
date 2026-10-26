# Retraduction 🌍🎮

Smart, offline, and resumable `gamelist.xml` translator for RetroBat and Batocera. This tool uses neural AI models to automatically translate your game descriptions without relying on external APIs, API keys, or request limits.

⚠️ **CRITICAL REQUIREMENT:** The original `gamelist.xml` descriptions **MUST** be in English. The program is specifically configured to translate from English to your selected target language.

## ✨ Features
* **100% Offline Translation:** Uses your CPU to translate locally (no API limits).
* **Auto-Resume:** Saves progress every 25 games. If you close the app or your PC restarts, it will automatically resume exactly where it left off!
* **Anti-Hallucination Filter:** Includes a safety mechanism to prevent the AI from entering infinite text loops (a common issue with AI translators).
* **Multi-Language UI:** The interface automatically detects your Windows language and adapts to English, Spanish, French, Italian, or Portuguese.
* **Non-Destructive:** It never overwrites your original file. It creates a new one (e.g., `gamelist_es.xml`).

## 🚀 How to Use

1. **Download** the `retraduction.exe` file and place it in the exact same folder as your English `gamelist.xml` (for example, inside your `roms/arcade` folder).
2. **Double-click** `retraduction.exe` to run it. No Python installation is required!
3. **Select your target language** from the interactive menu.
4. Let the program work. Once finished, you will get a new file (like `gamelist_es.xml`).
5. Keep your original file safe, and rename the new translated file to `gamelist.xml` so your frontend can read it.

## 📡 Important Note on the First Run
The **very first time** you select a specific target language, the program will need an active Internet connection for a few seconds to download the neural translation model to your local hard drive. 
Once the model is downloaded, all future translations for that language will be completely offline.

## 🛠️ Built With
* [Argos Translate](https://github.com/argosopentech/argos-translate) - Offline neural machine translation.
* [Rich](https://github.com/Textualize/rich) - Beautiful terminal formatting.
