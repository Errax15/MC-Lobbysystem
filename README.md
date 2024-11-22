# Lobbysystem für Minecraft (Spigot 1.21)

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
| `/lobby`            | 🇩🇪 Teleportiert den Spieler in die Lobby.           <br>🇺🇸 Teleports the player to the lobby. |
| `/spawn`            | 🇩🇪 Teleportiert den Spieler zum festgelegten Spawnpunkt.<br>🇺🇸 Teleports the player to the set spawn point. |

### 📌 Admin-Befehle / Admin Commands

| **Befehl/Command**   | **Beschreibung/Description**                          |
|-----------------------|------------------------------------------------------|
| `/setlobby`          | 🇩🇪 Setzt die aktuelle Position als Lobbypunkt.      <br>🇺🇸 Sets the current position as the lobby point. |
| `/setspawn`          | 🇩🇪 Setzt den aktuellen Standort als Spawnpunkt.     <br>🇺🇸 Sets the current location as the spawn point. |
| `/reloadlobby`       | 🇩🇪 Lädt die Plugin-Konfiguration neu.               <br>🇺🇸 Reloads the plugin configuration. |

---

## ⚙️ Configs

🇩🇪 | Die Konfigurationsdatei ermöglicht eine einfache Anpassung des Lobbysystems. Sie befindet sich unter:  
`/plugins/MC-Lobbysystem/config.yml`  
🇺🇸 | The configuration file allows for easy customization of the lobby system. It can be found at:  
`/plugins/MC-Lobbysystem/config.yml`

### Beispielkonfiguration / Example Configuration:

```yaml
lobby:
  location:
    x: 0
    y: 64
    z: 0
    world: world
spawn:
  location:
    x: 100
    y: 64
    z: 100
    world: world
messages:
  teleport-lobby: "Willkommen in der Lobby!"
  teleport-spawn: "Willkommen am Spawn!"
```

---

## 🔑 Permissions

🇩🇪 | Das Plugin nutzt folgende Berechtigungen:  
🇺🇸 | The plugin uses the following permissions:  

| **Permission**         | **Beschreibung/Description**                                 |
|-------------------------|------------------------------------------------------------|
| `lobby.use`            | 🇩🇪 Erlaubt Spielern, `/lobby` zu nutzen.                   <br>🇺🇸 Allows players to use `/lobby`. |
| `lobby.set`            | 🇩🇪 Erlaubt Admins, `/setlobby` zu nutzen.                  <br>🇺🇸 Allows admins to use `/setlobby`. |
| `spawn.use`            | 🇩🇪 Erlaubt Spielern, `/spawn` zu nutzen.                   <br>🇺🇸 Allows players to use `/spawn`. |
| `spawn.set`            | 🇩🇪 Erlaubt Admins, `/setspawn` zu nutzen.                  <br>🇺🇸 Allows admins to use `/setspawn`. |

---

## ✨ Authors

🇩🇪 | Dieses Plugin wurde von [Dein Name] entwickelt.  
🇺🇸 | This plugin was developed by [Your Name].  

🇩🇪 | Vielen Dank für die Nutzung des MC-Lobbysystems!  
🇺🇸 | Thank you for using the MC-Lobby system!

---

## 📧 Support

🇩🇪 | Bei Fragen oder Problemen, kontaktiere uns unter: [Deine E-Mail-Adresse]  
🇺🇸 | For questions or issues, contact us at: [Your Email Address]
