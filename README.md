![image](https://github.com/user-attachments/assets/6beee7d1-b531-48e8-b0e6-96f3922af252) 
---
![image](https://github.com/user-attachments/assets/79963724-1a18-4991-a3d3-e7ea587e3bce)

<h3 align = "center"> 
<img src="https://github.com/user-attachments/assets/5ddb695d-4ece-4ff2-8a98-22916db4c5a2" width="100" />
</p>

### <h3 align = "center">Downloads</p>
<h3 align="center">🇩🇪 Der Download zur Beta wird hier und auf Spigotmc.org verfügbar sein.</p>

<h3 align="center">🇺🇸 The download for the beta will be available here and on Spigotmc.org.</p>

---
<div align="center">
  <a href="https://github.com/users/Errax15/projects/1/views/1" target="_blank">
    <img src="https://img.shields.io/badge/github-Progress_Board-blue" alt="Progress Board" width="250" height="40">
  </a>
</div>

---

<h3 align = "center"><img src="https://github.com/user-attachments/assets/61bb771e-1c2a-4de8-bba4-ef60bea1fbe3" width="250" /></p>

<h3 align="center">🇩🇪 | Dieses Plugin bietet ein umfassendes Lobbysystem für Spigot-Server mit Version 1.21.</p>
<h3 align="center">🇺🇸 | This plugin provides a comprehensive lobby system for Spigot servers running version 1.21.</p>

---


<h3 align="center"><img src="https://github.com/user-attachments/assets/4b6737e4-ebb6-435f-a654-5c23a25b4dca" width="550" /></p>

### <h2 align="center">📌 Spielerbefehle / Player Commands</h2>

<h3>

| **Befehl/Command**  | **Beschreibung/Description**                          |
|----------------------|------------------------------------------------------|
| `/spawn`            | 🇩🇪 Teleportiert den Spieler zum festgelegten Spawnpunkt.<br>🇺🇸 Teleports the player to the set spawn point. |
| `/coins`            | 🇩🇪 Zeigt deine aktuellen Coins an.<br>🇺🇸 Displays your current coins. |
| `/coins see <player>`| 🇩🇪 Zeigt die Coins eines anderen Spielers an.<br>🇺🇸 Displays the coins of another player. |

</h3>

### <h2 align="center">📌 Admin-Befehle / Admin Commands</h2>

<h3>

| **Befehl/Command**   | **Beschreibung/Description**                          |
|-----------------------|------------------------------------------------------|
| `/setspawn`          | 🇩🇪 Setzt den aktuellen Standort als Spawnpunkt.     <br>🇺🇸 Sets the current location as the spawn point. |
| `/coins modify <player> <amount>` | 🇩🇪 Ändert die Coins eines anderen Spielers um den angegebenen Betrag.<br>🇺🇸 Modifies the coins of another player by the specified amount. |
| `/coins reset <player>` | 🇩🇪 Setzt die Coins eines anderen Spielers auf 0 zurück.<br>🇺🇸 Resets the coins of another player to 0. |

</h3>

<h3 align="center"><img src="https://github.com/user-attachments/assets/852e3f85-caef-4e70-aa07-2e01811d18fd" width="400" /></p>

🇩🇪 | Die Konfigurationsdatei ermöglicht eine einfache Anpassung des Lobbysystems. Sie befindet sich unter:  
`/plugins/Lobbysystem/config.yml`  
`/plugins/Lobbysystem/messages.yml`
`plugins/Lobbysystem/data/PlayerData.yml`

🇺🇸 | The configuration file allows for easy customization of the lobby system. It can be found at:  
`/plugins/Lobbysystem/config.yml`
`plugins/Lobbysystem/messages.yml`
`plugins/Lobbysystem/data/PlayerData.yml`

### <h3 align="center">Standart Konfiguration / Default Config:</p>

```yaml
# Plugin Configuration

# General
prefix: "§bLobby §8| "
Level: "2024"
HotbarSounds: true


# Welcome effects
welcome:
  title: §e✨ §5Willkommen! §e✨
  subtitle: §d🎉 §aViel Spaß und Erfolg! §c🚀
  title_enabled: true
  blindness_enabled: true
  sound_enabled: true
  blindness_duration: 45  # Duration of Blindness (1 second = 20 Ticks)

# Welcome messages
messages:
  firstjoin: "§6%player% §6ist zum ersten Mal auf dem Server! Willkommen!" # When the player joins the server for the first time, they receive a special join message.
  join: "§a%player% §aist der Lobby beigetreten."
  leave: "§c%player% §cchat die Lobby verlassen."

# Spawn
# (But it's Easy to use with /setspawn)
spawn:
  world: "world"
  x: 0.0
  y: 100.0
  z: 0.0
  yaw: 0.0
  pitch: 0.0

# Navigator general
CompassName: "§b§lNavigator"

# Navigator Items
navigator:
  item1:
    material: REDSTONE
    name: Teleport zu 0, 0, 0
    description: "Teleportiere dich zu den Koordinaten 0, 0, 0"
    slot: 13
    coordinates:
      x: 0
      y: 100
      z: 0

  item2:
    material: EMERALD
    name: Teleport zu 100, 64, 100
    description: "Teleportiere dich zu den Koordinaten 100, 64, 100"
    slot: 14
    coordinates:
      x: 100
      y: 64
      z: 100
  # add more...


# Gadgets
gadgetitemname: "§7§lGadgets"


# Köpfe
heads:
  - Errax15
  - NoRiskk
  - Paluten
  - BastiGHG
  - Spieler4
  - Spieler5
  - Spieler6
  - Spieler7



```

---

<h3 align="center"><img src="https://github.com/user-attachments/assets/5cfbb09e-de10-4ad3-83ed-d0a2fa21f141" width="700" /></p>

<h3 align="center">🇩🇪 | Das Plugin nutzt folgende Berechtigungen:  </p>
<h3 align="center">🇺🇸 | The plugin uses the following permissions:  </p>

### <h3 align="center">📌 Berechtigungen / Permissions</h3>

<h3>

| **Permission**         | **Beschreibung/Description**                                 |
|-------------------------|------------------------------------------------------------|
| `Lobbysystem.*`            | 🇩🇪 Erlaubt es alle Einrichtungsbefehle zu nutzen.                   <br>🇺🇸 Allows the use of all setup commands. |
| `Lobbysystem.admin`        | 🇩🇪 Erlaubt es fast alle Einrichtungsbefehle zu nutzen.       <br>🇺🇸 Allows the use almost of all setup commands. |
| `Lobbysystem.coins.modify` | 🇩🇪 Erlaubt dir /coins modify zu benutzen.                   <br>🇺🇸 Allows you to use /coins modify.              |
| `Lobbysystem.coins.reset`  | 🇩🇪 Erlaubt es alle Einrichtungsbefehle zu nutzen.                   <br>🇺🇸 Allows the use of all setup commands. |

</h3>

---

<h3 align="center"><img src="https://github.com/user-attachments/assets/5d0938ca-701a-409e-8639-af7618e16a96" width="500" /></p>

<h3 align="center">🇩🇪 | Dieses Plugin wurde von [Errax15] entwickelt.  </p>
<h3 align="center">🇺🇸 | This plugin was developed by [Errax15].  </p>

<h3 align="center">🇩🇪 | Vielen Dank für die Nutzung des Lobbysystems! </p> 
<h3 align="center">🇺🇸 | Thank you for using the Lobby system!</p>

---

<h3 align="center"><img src="https://github.com/user-attachments/assets/e958e1b8-eefa-491b-b96c-0ee5d383cdd3" width="500" /></p>
<h3 align="center"> 🇩🇪 | Bei Fragen oder Problemen, kontaktiere uns unter:<a href="https://github.com/Errax15/MC-Lobbysystem/issues" target="_blank"><img src="https://img.shields.io/badge/Lobbysystem-probleme-gold" alt="Issuegerman"></a></h3>
<h3 align="center"> 🇺🇸 | For questions or issues, contact us at:<a href="https://github.com/Errax15/MC-Lobbysystem/issues" target="_blank"><img src="https://img.shields.io/badge/Lobbysystem-issues-gold" alt="Issueenglish"></a></h3>
