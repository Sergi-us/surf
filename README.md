# 🌊 surf - Simple Browser

**Suckless Webbrowser für SARBS**

> **🔄 Umzug zu Codeberg**: Die aktive Entwicklung und Kollaboration findet jetzt auf [Codeberg](https://codeberg.org/Sergius/surf) statt. GitHub dient nur als Mirror.
> 
> **📦 Hauptprojekt**: [SARBS](https://codeberg.org/Sergius/SARBS) - [Homepage](https://sarbs.xyz/sarbs/)

Minimalistischer Webbrowser basierend auf WebKit2/GTK+ - fokussiert auf Tastatursteuerung und Scriptbarkeit.

## ✨ Features

### Kern-Funktionalität
- **WebKit2/GTK+** Engine - Moderne Webstandards
- **Minimalistisch** - Kein UI-Overhead, nur der Inhalt zählt
- **Tastatursteuerung** - Volle Navigation ohne Maus

### Erweiterte Features
- **XEmbed-Protokoll** - Einbettbar in andere Anwendungen (z.B. tabbed)
- **XProperties-Steuerung** - Externe Kontrolle via X Properties
- **Scriptbar** - Erweiterbar durch Shell-Skripte
- **Konfigurierbar** - Anpassbar über config.h

### Patches
- **surf-2.0-homepage** - Konfigurierbare Homepage

## ⚡ Installation

### Automatisch mit SARBS (empfohlen)
Wird durch das [SARBS-Installationsskript](https://codeberg.org/Sergius/SARBS) automatisch eingerichtet.

### Manuell
```bash
git clone https://codeberg.org/Sergius/surf.git
cd surf
sudo make install
```

### Abhängigkeiten
- `webkit2gtk` - WebKit Engine
- `gcr` - Gnome Crypto Library
- `glib-networking` - Netzwerk-Support
- `libX11` - X11 Library

## 🛠️ Nutzung

### Basis
```bash
# surf starten
surf https://sarbs.xyz

# Mit Tabs (benötigt tabbed)
tabbed -c surf -e
```

### Tastenkombinationen

Die wichtigsten Keybindings (siehe [config.h](config.h) für alle):

- `Ctrl+g` - URL-Leiste öffnen
- `Ctrl+f` - Suche
- `Ctrl+/` - Zurück
- `Ctrl+Shift+/` - Vorwärts
- `Ctrl+r` - Neu laden
- `Ctrl+Shift+r` - Cache leeren & neu laden
- `Ctrl+h/l` - Navigation (Vim-Style)

### Mit tabbed verwenden

Für Tab-Unterstützung zusammen mit [tabbed](https://codeberg.org/Sergius/tabbed):

```bash
tabbed -c surf -e
```

**Tipp**: In SARBS ist dies als Standard-Browser eingerichtet!

## 🎨 Konfiguration

Anpassungen in `config.h`:
- Startseite
- User Agent
- Keybindings
- Cookie-Policy
- JavaScript-Settings
- Und mehr...

Nach Änderungen:
```bash
sudo make clean install
```

## 🔧 Erweiterte Features

### Skripte & Erweiterungen

surf kann durch Skripte erweitert werden. Siehe Beispiele im [surf-scripts Repository](https://github.com/felixr/surf-scripts).

### Ad-Blocking

Mit [surf-adblock](https://github.com/jun7/surf-adblock) oder durch manuelle Skripte.

## 📚 Weitere SARBS-Komponenten

- **[SARBS Hauptprojekt](https://codeberg.org/Sergius/SARBS)** - Auto-Rice Bootstrapping
- **[dotfiles](https://codeberg.org/Sergius/dotfiles)** - Konfigurationsdateien
- **[dwm](https://codeberg.org/Sergius/dwm)** - Window Manager
- **[st](https://codeberg.org/Sergius/st)** - Terminal Emulator
- **[dmenu](https://codeberg.org/Sergius/dmenu)** - Application Launcher
- **[tabbed](https://codeberg.org/Sergius/tabbed)** - Tab Interface für surf

## 🤝 Credits

- **[suckless.org](https://surf.suckless.org/)** - Original surf
- **WebKit Team** - WebKit Engine

## 📄 Lizenz

Siehe [LICENSE](LICENSE) Datei.

---

**📧 Kontakt**:
- [Codeberg Issues](https://codeberg.org/Sergius/surf/issues)
- [GitHub Issues](https://github.com/Sergi-us/surf/issues) (Mirror)
- [SARBS Homepage](https://sarbs.xyz/kontakt/)
