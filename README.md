<h3 align="center">🚧 Upcoming Update Notice 🚧</h3> <p align="center"> <strong>I’m already working on Update 1.0.4 daily, and I will continue to focus on it over the coming weeks to deliver a fully functional and complete lobby for you.<br><br> The listed features will be added to the progress board under version 1.0.4. Please be patient for a few more weeks.</strong><br><br> From time to time, test versions will be released, allowing you to try out features in advance.<br> <strong>Please note that these are unfinished versions, and we cannot take responsibility for any issues or potential damage that may occur during their use.</strong> </p>

<h3 align="center">❗️NEW UPDATE 1.0.3 ❗️</h3>

![image](https://github.com/user-attachments/assets/6beee7d1-b531-48e8-b0e6-96f3922af252)

---

<h3 align = "center"><img src="https://github.com/user-attachments/assets/32b24979-96b2-495c-a19a-dd62d67fe768" width="650" /></h3>

<div align="center">
  <a href="https://github.com/Errax15/MC-Lobbysystem/releases/latest" target="_blank">
    <img src="https://img.shields.io/badge/Plugin-Releases-gold" alt="Release Latest" width="220" height="40">
  </a>
</div>

---

<h3 align = "center"><img src="https://github.com/user-attachments/assets/61bb771e-1c2a-4de8-bba4-ef60bea1fbe3" width="250" /></h3>

<h3 align="center">🇩🇪 | Dieses Plugin bietet ein umfassendes Lobbysystem für Spigot-Server mit Version 1.21.</h3>
<h3 align="center">🇺🇸 | This plugin provides a comprehensive lobby system for Spigot servers running version 1.21.</h3>

---

<h3 align = "center"><img src="https://github.com/user-attachments/assets/85098738-b129-4b1c-a58e-bb5b72e073d0" width="550" /></h3>
<div align="center">
  <a href="https://github.com/users/Errax15/projects/1/views/1" target="_blank">
    <img src="https://img.shields.io/badge/github-Progress_Board-blue" alt="Progress Board" width="200" height="32">
  </a>
</div>

---

<h3 align="center"><img src="https://github.com/user-attachments/assets/4b6737e4-ebb6-435f-a654-5c23a25b4dca" width="550" /></h3>

### <h2 align="center">📌 Spielerbefehle / Player Commands</h2>

<div align="center">

<h3>

| **Befehl/Command**  | **Beschreibung/Description**                          |
|----------------------|------------------------------------------------------|
| `/spawn`            | 🇩🇪 Teleportiert den Spieler zum festgelegten Spawnpunkt.<br>🇺🇸 Teleports the player to the set spawn point. |
| `/coins`            | 🇩🇪 Zeigt deine aktuellen Coins an.<br>🇺🇸 Displays your current coins. |
| `/coins see <player>`| 🇩🇪 Zeigt die Coins eines anderen Spielers an.<br>🇺🇸 Displays the coins of another player. |

</h3>

</div>

### <h2 align="center">📌 Admin-Befehle / Admin Commands</h2>

<div align="center">

<h3>

| **Befehl/Command**   | **Beschreibung/Description**                          |
|-----------------------|------------------------------------------------------|
| `/setspawn`          | 🇩🇪 Setzt den aktuellen Standort als Spawnpunkt.     <br>🇺🇸 Sets the current location as the spawn point. |
| `/coins modify <player> <amount>` | 🇩🇪 Ändert die Coins eines anderen Spielers um den angegebenen Betrag.<br>🇺🇸 Modifies the coins of another player by the specified amount. |
| `/coins reset <player>` | 🇩🇪 Setzt die Coins eines anderen Spielers auf 0 zurück.<br>🇺🇸 Resets the coins of another player to 0. |

</h3>

</div>

---

<h3 align="center"><img src="https://github.com/user-attachments/assets/852e3f85-caef-4e70-aa07-2e01811d18fd" width="400" /></h3>

🇩🇪 | Die Konfigurationsdatei ermöglicht eine einfache Anpassung des Lobbysystems. Sie befindet sich unter:  
`/plugins/Lobbysystem/config.yml`  
`/plugins/Lobbysystem/messages.yml`
`/plugins/Lobbysystem/data/PlayerData.yml`

🇺🇸 | The configuration file allows for easy customization of the lobby system. It can be found at:  
`/plugins/Lobbysystem/config.yml`
`/plugins/Lobbysystem/messages.yml`
`/plugins/Lobbysystem/data/PlayerData.yml`

### <h2 align="center">Standart Konfiguration / Default Config:</h2>

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

scoreboard:
  title: "&b&l    DeinServer    &l"
  lines:
    - " "
    - "&a&lName"
    - "&7%player_name%"
    - "  "
    - "&6&lCoins"
    - "&e%coins%"
    - "   "

# Navigator general
CompassName: "§b§lNavigator"

# Navigator Items
navigator:
  use_bungeecord: true
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

<h3 align="center"><img src="https://github.com/user-attachments/assets/5cfbb09e-de10-4ad3-83ed-d0a2fa21f141" width="700" /></h3>

<h3 align="center">🇩🇪 | Das Plugin nutzt folgende Berechtigungen:  </h3>
<h3 align="center">🇺🇸 | The plugin uses the following permissions:  </h3>
<h3>
<div align="center">

| **Permission**                     | **Beschreibung/Description**                                                                 |
|-------------------------------------|--------------------------------------------------------------------------------------------|
| `Lobbysystem.*`                    | 🇩🇪 Erlaubt es alle Einrichtungsbefehle zu nutzen.                                           <br>🇺🇸 Allows the use of all setup commands. |
| `Lobbysystem.admin`                | 🇩🇪 Erlaubt es fast alle Einrichtungsbefehle zu nutzen.                                      <br>🇺🇸 Allows the use almost of all setup commands. |
| `Lobbysystem.coins.modify`         | 🇩🇪 Erlaubt dir /coins modify zu benutzen.                                                  <br>🇺🇸 Allows you to use /coins modify.              |
| `Lobbysystem.coins.reset`          | 🇩🇪 Erlaubt es alle Einrichtungsbefehle zu nutzen.                                           <br>🇺🇸 Allows the use of all setup commands. |
| `Lobbysystem.gadgets.*`            | 🇩🇪 Erlaubt Zugriff auf alle Gadgets.                                                       <br>🇺🇸 Allows access to all gadgets. |
| `Lobbysystem.gadgets.enterhaken`   | 🇩🇪 Erlaubt Zugriff auf das Enterhaken Gadget.                                              <br>🇺🇸 Allows access to the grappling hook gadget. |
| `Lobbysystem.gadgets.elytra`       | 🇩🇪 Erlaubt Zugriff auf das Elytra Gadget.                                                  <br>🇺🇸 Allows access to the Elytra gadget. |
| `Lobbysystem.gadgets.catbazooka`   | 🇩🇪 Erlaubt Zugriff auf das Katzenbazooka Gadget.                                           <br>🇺🇸 Allows access to the Cat Bazooka gadget. |
| `Lobbysystem.gadgets.paintballgun` | 🇩🇪 Erlaubt Zugriff auf das Paintballgun Gadget.                                            <br>🇺🇸 Allows access to the Paintball Gun gadget. |
| `Lobbysystem.gadgets.sitonplayer`  | 🇩🇪 Erlaubt Zugriff auf das SitonPlayer Gadget.                                             <br>🇺🇸 Allows access to the Sit on Player gadget. |

</div>
</h3>

---

<h3 align="center"><img src="https://github.com/user-attachments/assets/5d0938ca-701a-409e-8639-af7618e16a96" width="500" /></h3>

<h3 align="center">🇩🇪 | Dieses Plugin wurde von [Errax15] entwickelt.  </h3>
<h3 align="center">🇺🇸 | This plugin was developed by [Errax15].  </h3>

<h3 align="center">🇩🇪 | Vielen Dank für die Nutzung des Lobbysystems! </h3> 
<h3 align="center">🇺🇸 | Thank you for using the Lobby system!</h3>

---

<h3 align="center"><img src="https://github.com/user-attachments/assets/e958e1b8-eefa-491b-b96c-0ee5d383cdd3" width="500" /></h3>
<h3 align="center"> 🇩🇪 | Bei Fragen oder Problemen, kontaktiere uns unter:<a href="https://github.com/Errax15/MC-Lobbysystem/issues" target="_blank"><img src="https://img.shields.io/badge/Lobbysystem-probleme-gold" alt="Issuegerman"></a></h3>
<h3 align="center"> 🇺🇸 | For questions or issues, contact us at:<a href="https://github.com/Errax15/MC-Lobbysystem/issues" target="_blank"><img src="https://img.shields.io/badge/Lobbysystem-issues-gold" alt="Issueenglish"></a></h3>

---

<h3 align="center"><img src="https://github.com/user-attachments/assets/ad86f33b-98c3-4228-9f27-a9e372e06f71" width="500" /></h3>

Developed by Errax15
