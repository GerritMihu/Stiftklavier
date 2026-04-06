# Stiftklavier – Aufbauanleitung

**Schritt-für-Schritt-Anleitung für den Aufbau des Stiftklaviers (Stylophone).**
🎯 **Ziel**: Ein funktionierendes, musikalisches Lehrmittel für Elektronik und Mechatronik.

---
## ⚠️ Wichtige Hinweise
> **Sicherheit & Qualität**
> - **IC-Orientierung prüfen**: Pin 1 ist mit einem Punkt markiert.
> - **Nur die großen Kupferflächen mit dem Stift berühren** – andere Bereiche können die Transistoren/ICs beschädigen.
> - **Lötstellen kontrollieren**: Keine Kurzschlüsse oder Kaltlötstellen!

---
## 📋 Material & Werkzeuge
### **Benötigte Komponenten** (siehe [BOM](bom/))
| Komponente          | Menge | Hinweise                                  |
|----------------------|-------|-------------------------------------------|
| Widerstände          | 12x   | Werte nach Schaltplan (ggf. parallel/seriell kombinieren) |
| IC (z. B. 555-Timer)  | 1x    | **Achtung**: Pin 1 markieren!             |
| Potentiometer 1k/50k | 2x    | 1k für Tonhöhe, 50k für Lautstärke         |
| Lautsprecher         | 1x    | Polung beachten (siehe Schritt 3)         |
| 9V-Blockbatterie     | 1x    | Frisch und voll geladen                   |
| Kabel (0,2 mm²)      | 10x   | 4x rot (120 mm), 6x schwarz (120 mm)       |

### **Werkzeuge**
- Lötkolben + Lötzinn
- Multimeter (für Widerstandsprüfung)
- Seitenschneider + Abisolierzange
- 5,5 mm-Bohrer (für Potentiometer-Löcher)

---
## 🔧 Aufbau – Schritt für Schritt

### **1. Platine bestücken**
**Ziel**: Alle SMD-/Durchsteckkomponenten korrekt platzieren.
1. **Beginne mit den kleinsten Bauteilen** (Widerstände, Dioden, dann IC).
2. **Widerstände**:
   - Werte **exakt** nach Schaltplan wählen.
   - Falls nötig, Widerstände **parallel/seriell kombinieren** (z. B. 2x 10k → 5k).
3. **IC einlöten**:
   - **Pin 1** (markiert) **nach links oben** ausrichten.
   - **Prüfen**: Multimeter auf Durchgang – keine Kurzschlüsse zwischen Pins!

---
### **2. Kabel vorbereiten**
**Ziel**: 10 Kabel mit korrekter Länge und Abisolierung.
| Farbe  | Länge | Menge | Verwendung                  |
|--------|-------|-------|-----------------------------|
| Rot    | 120mm | 4x    | Stromversorgung/Buttons     |
| Schwarz| 120mm | 6x    | Masse/Potentiometer         |
| Rot    | 230mm | 1x    | Lautsprecher (+)           |
| Schwarz| 230mm | 2x    | Lautsprecher (–)/Stylus    |

**Schritte**:
1. Kabel auf Länge schneiden.
2. **10 mm abisolieren** (beidseitig).
3. **Lötzinn vorverzinnen** für bessere Verbindungen.

---
### **3. Lautsprecher anlöten**
**Ziel**: Stabile Verbindung für klare Tonwiedergabe.
1. **230 mm-Kabel** (rot/schwarz) an Lautsprecher löten.
   - **Polarität**: Rot = **+**, Schwarz = **–** (für gleiche Phasenlage bei mehreren Lautsprechern).
   - **Tipp**: Autolötpaste für bessere Haftung auf Metall verwenden.
2. **Prüfen**: Widerstandsmessung (sollte ~8 Ω sein).

---
### **4. Potentiometer vorbereiten**
**Ziel**: 1k- und 50k-Poti für Tonhöhe/Lautstärke einbauen.
1. **Schwarze Kabel** (120 mm) an **alle 3 Pins** jedes Potis löten.
2. **Positionieren**:
   - **1k-Poti**: Neben Lautsprecher (3 Löcher in Reihe).
   - **50k-Poti**: Andere Seite der Platine (3 Löcher).

---
### **5. Komponenten auf Platine löten**
**Ziel**: Alle vorbereiteten Teile (Lautsprecher, Potis, Batterieclip) anlöten.
- **Lautsprecher**: Auf der **Button-gegenüberliegenden Seite**.
- **Batterieclip**: Rot = **unten** (zu den Kupferflächen).
- **Stylus-Kabel**: 230 mm-Kabel an **einzelnes Loch nahe Diode** löten (anderes Ende später).

---
### **6. Erste Inbetriebnahme**
1. **Sichtprüfung**: Alle Lötstellen auf Kaltlötstellen/Kurzschlüsse prüfen.
2. **IC-Orientierung doppelt checken** (Pin 1!).
3. **9V-Batterie anschließen** – beide Buttons drücken → Ton sollte hörbar sein.

---
### **7. Gehäuse bearbeiten**
**Ziel**: 3D-gedrucktes Gehäuse für Potentiometer und Stylus anpassen.
1. **Bohrungen**:
   - **5,5 mm-Loch** für 1k-Poti **vergrößern** (existierendes Loch).
   - **Neues 5,5 mm-Loch** 20 mm rechts daneben bohren (für 50k-Poti).
   - **5 mm-Loch** für Stylus-Aufbewahrung (siehe [Abbildung 2](bilder/Abbildung2.png)).
2. **Potentiometer montieren**:
   - Von **innen** mit Heißkleber fixieren (nicht den Drehknopf verkleben!).
3. **Schraubmuttern einsetzen**:
   - **Heat-Set-Muttern** in die hinteren Löcher drücken und mit Lötkolben fixieren.

---
### **8. Platine einbauen**
1. Platine **horizontal von hinten** ins Gehäuse schieben (Kupferflächen nach vorne).
2. **9V-Batterie** unter der Platine platzieren.

---
### **9. Stylus vorbereiten**
**Ziel**: 100 mm-Kupferdraht (6 mm²) als Stift für die Tonabnahme.
1. **Ein Ende rund feilen**.
2. **15 mm abisolieren** und an das 230 mm-Kabel löten.
3. **Shrink-Tube** (40 mm) über die Lötstelle schieben und erhitzen.

---
### **10. Buttons anbringen**
- **Beide Buttons gleichzeitig drücken** → Ton erzeugt.
- **Deckel aufschrauben** (vorher Buttons durch die Löcher stecken).

---
## 🔍 Troubleshooting
| Problem                | Ursache                          | Lösung                                  |
|------------------------|----------------------------------|----------------------------------------|
| **Kein Ton**           | Falsche IC-Orientierung          | Pin 1 prüfen, ggf. umlöten             |
| **Verzerrter Klang**   | Kaltlötstelle am Lautsprecher    | Nachlöten, Widerstand prüfen           |
| **Buttons reagieren nicht** | Unterbrochene Kabel          | Durchgang prüfen, neu löten            |

---
## 📚 Weiterführendes
- [Schaltplan (PDF)](cam/Stylophon_1.pdf)
- [3D-Modelle für Gehäuse](3D/)
- [BOM mit Bestelllinks](bom/)

---
**Fertig!** 🎉
→ Experimentiere mit anderen Widerständen für neue Tonleitern oder baue ein MIDI-Interface ein.