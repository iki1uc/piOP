# piOP – ROOT ONLINE SYSTEM V9

Das Projekt **piOP** enthält das ROOT‑ONLINE‑V9‑System.  
Es simuliert einen geschützten Zustand mit Fehlerphasen, Rücksprungmechanismen und einem interaktiven Schutzsystem.

---

## 🎯 Zweck des Systems

Das ROOT‑ONLINE‑V9‑Modul dient als:

- Fehler‑Simulator  
- Schutz‑Mechanismus‑Tester  
- Zustand‑Lader (root.state)  
- Interaktive Sicherheitslogik  

Es ist vollständig clientseitig und benötigt keine Server‑Komponenten.

---

## 📁 Dateien im Repository

| Datei | Funktion |
|-------|----------|
| `index.html` | Hauptsystem, UI, Logik, Schutzmechanismen |
| `root.state` | Externer Zustand (ROOT, E8, E16) |
| `README.md` | Dokumentation |

---

## 🧬 Struktur von `root.state`

Die Datei besteht aus **3 Zeilen**:

1. **ROOT** – eine einzelne Zahl  
2. **E8** – genau 8 Ziffern (0/1)  
3. **E16** – genau 16 Ziffern (0/1)

Beispiel:

1
01010101
0000111100001111


---

## 🔧 Schutzmechanismus

Der Schutz aktiviert sich, wenn:

- **Phase‑1‑Fehler ≥ 4**  
- **Phase‑2‑Fehler ≥ 3**

Ablauf:

1. 3 Sekunden warten  
2. Taste drücken  
3. 3 Treffer klicken  
4. Schutz bestanden → System läuft weiter  
5. Schutz nicht bestanden → Rücksprung (`MODI_ALT`)

---

## 📌 Status

Das System ist stabil, modular und bereit für Erweiterungen.

# piOP – ROOT ONLINE V9

Dieses Projekt enthält das ROOT‑ONLINE‑V9‑System:

- Ladefunktion für `root.state`
- Fehlerphasen‑Simulation
- Schutzmechanismus mit Interaktion
- Rücksprung in alten Zustand

`root.state` muss 3 Zeilen enthalten:

