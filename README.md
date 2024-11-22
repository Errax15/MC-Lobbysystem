# Lobbysystem für Minecraft (Spigot 1.21)

# BETA RELEASE 01.12.2024 0:00

⏳ Der Countdown läuft...

```html
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BETA RELEASE Countdown</title>
    <script>
        // Set the date we're counting down to
        var countDownDate = new Date("Dec 1, 2024 00:00:00").getTime();

        // Update the countdown every 1 second
        var x = setInterval(function() {
            // Get the current date and time
            var now = new Date().getTime();

            // Find the time remaining
            var distance = countDownDate - now;

            // Time calculations for days, hours, minutes, and seconds
            var days = Math.floor(distance / (1000 * 60 * 60 * 24));
            var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
            var seconds = Math.floor((distance % (1000 * 60)) / 1000);

            // Display the result in an element with id="countdown"
            document.getElementById("countdown").innerHTML = days + "T " + hours + "h " + minutes + "m " + seconds + "s ";

            // If the countdown is over, display a message
            if (distance < 0) {
                clearInterval(x);
                document.getElementById("countdown").innerHTML = "BETA RELEASE IST JETZT!";
            }
        }, 1000);
    </script>
</head>
<body>
    <h1>BETA RELEASE Countdown</h1>
    <p id="countdown"></p>
</body>
</html>
```
🇩🇪 | Dieses Plugin bietet ein umfassendes Lobbysystem für Spigot-Server mit Version 1.21.  
🇺🇸 | This plugin provides a comprehensive lobby system for Spigot servers running version 1.21.

---

## 📄 Info

🇩🇪 | Das MC-Lobbysystem wurde speziell entwickelt, um Serveradministratoren zu unterstützen, eine benutzerfreundliche Lobby-Umgebung zu schaffen. Es bietet Funktionen wie benutzerdefinierte Befehle, Konfigurationen und erweiterte Berechtigungen.  
🇺🇸 | The MC-Lobby system is designed to help server administrators create a user-friendly lobby environment. It offers features such as custom commands, configurations, and advanced permissions.

---

## 🛠️ Commands

### 📌 Spielerbefehle / Player Commands

| **Befehl/Command** | **Beschreibung/Description**                          |
|---------------------|------------------------------------------------------|
| `/spawn`            | 🇩🇪 Teleportiert den Spieler zum festgelegten Spawnpunkt.<br>🇺🇸 Teleports the player to the set spawn point. |

### 📌 Admin-Befehle / Admin Commands

| **Befehl/Command**   | **Beschreibung/Description**                          |
|-----------------------|------------------------------------------------------|
| `/setspawn`          | 🇩🇪 Setzt den aktuellen Standort als Spawnpunkt.     <br>🇺🇸 Sets the current location as the spawn point. |

---

## ⚙️ Configs

🇩🇪 | Die Konfigurationsdatei ermöglicht eine einfache Anpassung des Lobbysystems. Sie befindet sich unter:  
`/plugins/Lobbysystem/config.yml`  
`/plugins/Lobbysystem/messages.yml`
`plugins/Lobbysystem/data/PlayerData.yml`
🇺🇸 | The configuration file allows for easy customization of the lobby system. It can be found at:  
`/plugins/Lobbysystem/config.yml`
`plugins/Lobbysystem/messages.yml`
`plugins/Lobbysystem/data/PlayerData.yml`
### Standart Konfiguration / Default Config:

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

## 🔑 Permissions

🇩🇪 | Das Plugin nutzt folgende Berechtigungen:  
🇺🇸 | The plugin uses the following permissions:  

| **Permission**         | **Beschreibung/Description**                                 |
|-------------------------|------------------------------------------------------------|
| `Lobbysystem.admin`            | 🇩🇪 Erlaubt es alle Einrichtungsbefehle zu nutzen.                   <br>🇺🇸 Allows the use of all setup commands. |


---

## ✨ Authors

🇩🇪 | Dieses Plugin wurde von [Errax15] entwickelt.  
🇺🇸 | This plugin was developed by [Errax15].  

🇩🇪 | Vielen Dank für die Nutzung des Lobbysystems!  
🇺🇸 | Thank you for using the Lobby system!

---

## 📧 Support

🇩🇪 | Bei Fragen oder Problemen, kontaktiere uns unter: [Github Issues](https://github.com/Errax15/MC-Lobbysystem/issues)
🇺🇸 | For questions or issues, contact us at: [Github Issues](https://github.com/Errax15/MC-Lobbysystem/issues)
