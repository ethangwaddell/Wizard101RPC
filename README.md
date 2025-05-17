# 🧙‍♂️ Wizard101RPC

Wizard101RPC is a tool that adds **Discord Rich Presence** support to Wizard101.

![Wizard101RPC](https://media.discordapp.net/attachments/1230704557093425185/1373047039503368242/image.png?ex=6828fd34&is=6827abb4&hm=f56b2b3c966452c1323fa89b38a4902bb38520c61178a1f1f6864a6a32e49cce&=&format=webp&quality=lossless)

### Features

* **Live Discord Rich Presence**
  Displays your current zone, health, quest, and combat status while playing Wizard101.

* **Combat Awareness**
  Detects when you're in battle and shows the name of the enemy you're fighting.

* **Quest and Zone Tracking**
  Automatically updates with active quests and your location in the Spiral using up-to-date data.

* **Tray Icon and Background Operation**
  Runs silently in the background with a system tray icon and exit option.

* **Auto-Updating**
  Checks for new versions and updates itself from the latest GitHub release.
  
---

### Installation

1. Download the latest `.exe` from the [Releases](https://github.com/ethangwaddell/Wizard101RPC/releases) page.
2. Run the file — no installation required.
3. On first launch, select your Wizard101 installation path.
4. Wizard101RPC runs in the background and updates Discord presence automatically.

---

### Requirements

* Windows 10 or 11
* Discord desktop client (Rich Presence does not show in browser)
* Wizard101 (Windows or Steam version)

---

### Auto-Updating

The application checks for new releases on startup and replaces itself with the latest version automatically when available.

---

### How It Works

* Monitors the `WizardClient.log` file in real time
* Parses game state: zone, quest, combat, health
* Uses maintained and daily updated `.json` files to map enemies, quests, and zones
* Updates Discord Rich Presence using the `pypresence` library

---

### Known Limitations

* Some data may fail to load temporarily due to rate limits, but will soon.

---

### AppData Location

All configuration and JSON data is stored in:

```
%APPDATA%\Wizard101RPC
```

This includes:

* `config.json`
* `Enemies.json`
* `Quests.json`
* `Zones.json`

---

### License

This project is open source under the MIT License.
