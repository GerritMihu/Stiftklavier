# Stiftklavier / Stylophone

**Ein Open-Source-Lehrprojekt für Mechatronik, Elektronik und Musik** – ideal für Workshops, Schulen und Maker.

![Stiftklavier-Prototyp](bilder/Stiftklavier_Fertig.jpg)
*(Abb.: Fertiger Aufbau mit 3D-gedrucktem Gehäuse)*

---
## 🎯 Projektziel
Das Stiftklavier ist ein **praktisches Lehrmittel**, um:
✅ **Löten und Schaltungen** zu üben (Widerstände, ICs, Transistoren)
✅ **Grundlagen der Tonerzeugung** zu verstehen (Oszillatoren, Filter)
✅ **Mechatronik** zu verbinden (Elektronik + 3D-Druck + Mechanik)
✅ **Kreativität** zu fördern (individuelle Gehäuse, Sound-Experimente)

**Zielgruppe**: Student:innen, Lehrende, Elektronik-Enthusiast:innen

---
## 📦 Inhalte dieses Repos
| Ordner/Datei          | Beschreibung                                  |
|-----------------------|-----------------------------------------------|
| [`3D/`](3D/)          | 3D-Modelle für Gehäuse (STL, FreeCAD)         |
| [`bom/`](bom/)        | Stücklisten (BOM) und Bestelllinks           |
| [`cam/`](cam/)        | **Automatisch generierte KiBot-Exporte** (PDF/PNG/3D) |
| [`Stylophone Documentation.md`](Stylophone%20Documentation.md) | **Detaillierte Aufbauanleitung** 🔗 |
| [`Stylophon_1.kicad_sch`](Stylophon_1.kicad_sch) | KiCad-Schaltplan und Platinenlayout |

---
## 🛠️ Loslegen
### 1. Material besorgen
- [Stückliste (BOM)](bom/) mit empfohlenen Händlern.
- **Werkzeuge**: Lötkolben, Multimeter, 3D-Drucker (optional).

### 2. Aufbauen
→ **[Schritt-für-Schritt-Anleitung](Stylophone%20Documentation.md)**

### 3. Erweitern
- Experimentiere mit **anderen Widerständen** für neue Tonleitern.
- Baue ein **MIDI-Interface** ein (Code-Beispiele folgen).

---
## 🔧 CI/CD mit KiBot (KiCad 10 Docker)
Dieses Repo nutzt **[KiBot](https://github.com/INTI-CMNB/KiBot)** in einem **vorkonfigurierten Docker-Container für KiCad 10**, um automatisch:
- **Schaltpläne als PDF** zu exportieren
- **Platinen-Layouts als PNG** zu rendern
- **3D-Ansichten** der Platine zu generieren

👉 **Ergebnisse**: Siehe [`cam/`](cam/)-Ordner (automatisch aktualisiert bei Pushs).

---
## 🤝 Mitwirken
- **Fehler gefunden?** → [Issue erstellen](https://github.com/GerritMihu/Stiftklavier/issues)
- **Verbesserungen?** → Pull Requests willkommen!
- **Fragen?** → Diskussionsbereich nutzen.

---
## 📄 Lizenz
[MIT](LICENSE) – Nutze, modifiziere und teile das Projekt frei!

<!-- KiBot Docker Pipeline Test Trigger: $(date +%s) -->