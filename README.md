# 🏠 My Home Assistant Blueprints Collection

This repository is a collection of my custom Blueprints for Home Assistant. They are optimized for reliability and deep integration with **Synology**, **FritzBox**, and system monitoring.

## 📖 Overview
This repository serves as my central hub for Home Assistant Blueprints. 
Instead of maintaining complex automations on multiple devices, I use these templates 
to ensure a consistent and updateable setup across my smart home.

---

## 🚀 Available Blueprints

| Blueprint Name | Import | Version | Description |
| :--- | :--- | :--- | :--- |
| [📸 Synology Alarm Snapshot](./HomeAssistant/Blueprints/Automation/syno_alarm_snapshot.yaml) | <a href="https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/Cavekeeper/Home-Assistant-Blueprints/main/HomeAssistant/Blueprints/syno_alarm_snapshot.yaml"><img src="https://my.home-assistant.io/badges/blueprint_import.svg" width="160"></a> | v1.1.0 | Snapshot notification for Surveillance Station alarms. |
| [📸 Smart Light – Trigger](./HomeAssistant/Blueprints/Automation/smartlight_trigger.yaml) | <a href="https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/Cavekeeper/Home-Assistant-Blueprints/main/HomeAssistant/Blueprints/smartlight_trigger.yaml"><img src="https://my.home-assistant.io/badges/blueprint_import.svg" width="160"></a> | v1.0.1 | Stable motion-activated light automation. |
| [📸 Smart Shading: ON](./HomeAssistant/Blueprints/Automation/smart_rollershutter_shading_on.yaml) | <a href="https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/Cavekeeper/Home-Assistant-Blueprints/main/HomeAssistant/Blueprints/smart_rollershutter_shading_on.yaml"><img src="https://my.home-assistant.io/badges/blueprint_import.svg" width="160"></a> | v1.0.2 | The roller shutter lowers for shading when all conditions are met. It only runs once a day. |
| [📸 Smart Shading: OFF](./HomeAssistant/Blueprints/Automation/smart_rollershutter_shading_off.yaml) | <a href="https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/Cavekeeper/Home-Assistant-Blueprints/main/HomeAssistant/Blueprints/smart_rollershutter_shading_off.yaml"><img src="https://my.home-assistant.io/badges/blueprint_import.svg" width="160"></a> | v1.0.2 | Raises the roller shutter if the azimuth is exceeded OR the elevation is not reached. |
| *More coming soon...* | | | |

---

## 🛠 Installation

To import a blueprint into your Home Assistant instance:

1. **Find the Blueprint:** Go to the `HomeAssistant/Blueprints/` folder and click on the desired `.yaml` file.
2. **Get Raw Link:** Click the **"Raw"** button in the top right corner of the file view and copy the browser URL.
3. **Import:** In Home Assistant, navigate to **Settings** > **Automations & Scenes** > **Blueprints**.
4. Click **Import Blueprint**, paste the URL, and click **Preview / Import**.

<details>
<summary>⚖️ Legal & Technical Disclaimer (Click to expand)</summary>

---

## ⚠️ Disclaimer
**Use at your own risk.** These blueprints are designed for my personal home automation environment. While I strive for reliability, please note:
* **Storage:** Ensure that the file paths (e.g., for snapshots) exist on your system before running the automations.
* **Hardware:** Optimized for Raspberry Pi 4/5 and Synology DSM 7.x.
* **Privacy:** These scripts handle camera snapshots. Ensure your local storage is secured.
* **No Liability:** I am not responsible for any data loss, SD card wear, or security issues resulting from the use of these templates.


</details>

---

## 📖 Detailed Documentation

### 📸 Synology Alarm Snapshot
**File Path:** `HomeAssistant/Blueprints/syno_alarm_snapshot.yaml`

This blueprint bridges Synology Surveillance Station with Home Assistant notifications to provide instant visual security alerts.

* **Key Features:** Instant snapshots, mobile push notifications, and alarm panel integration.
* **Requirements:** Synology DSM Integration, HA Companion App.
* **Main Inputs:** Camera entity, motion counter, and push script.

---

## 💾 System Context & Setup
My local environment consists of:
* **Core:** Home Assistant running on a **Raspberry Pi**.
* **Database:** External **MariaDB** hosted on a **Synology NAS** (to protect the SD card and increase performance).
* **Network:** Managed via **FritzBox** integration.

---
*Created with ❤️ for a smarter home.*
