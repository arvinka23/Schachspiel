# Schachspiel

Ein vollstaendiges Schachspiel im Browser, entwickelt mit purem HTML, CSS und JavaScript -- ohne externe Frameworks oder Bibliotheken.

**Live-Demo:** [arvinka23.github.io/Schachspiel](https://arvinka23.github.io/Schachspiel/)

---

## Features

### Spielregeln
- Vollstaendige Zugvalidierung fuer alle Figurentypen
- Schach-, Schachmatt- und Patt-Erkennung
- Spezialzuege: **Rochade** (kurz & lang), **En Passant**, **Bauernumwandlung**
- Remis-Erkennung: 50-Zuege-Regel, dreifache Stellungswiederholung, ungenuegendes Material

### Bedienung
- **Klick** oder **Drag & Drop** zum Ziehen
- **Tastatursteuerung** (Pfeiltasten, Enter, Escape)
- Hervorhebung gueltiger Zuege und Schlagfelder
- Anzeige des letzten Zuges und Schach-Warnung mit Animation

### Funktionen
- Schachuhr (10 Minuten pro Spieler)
- Zughistorie in algebraischer Notation (Seitenleiste)
- Geschlagene Figuren mit Materialvorteil-Anzeige
- Zug zuruecknehmen (Undo)
- Brett drehen (Flip)
- PGN-Export in die Zwischenablage
- Aufgeben mit Bestaetigungsdialog
- Soundeffekte (ein-/ausschaltbar)

### Technik
- Responsives Design (Desktop & Mobile)
- Barrierefreiheit (ARIA-Labels, Tastaturnavigation, Fokus-Management)
- Modernes dunkles Theme mit CSS-Variablen
- Keine Abhaengigkeiten, laeuft direkt im Browser

---

## Projektstruktur

```
docs/
  index.html    – HTML-Struktur und Modals
  style.css     – Design, Layout, Animationen
  pieces.js     – Figurendefinitionen, Startposition, Hilfsfunktionen
  app.js        – Komplette Spiellogik (ChessGame-Klasse)
  tests.html    – Unit-Tests (im Browser ausfuehrbar)
```

---

## Lokale Ausfuehrung

Keine Installation noetig. Einfach `docs/index.html` im Browser oeffnen:

```bash
# Variante 1: Direkt oeffnen
open docs/index.html        # macOS
start docs/index.html       # Windows

# Variante 2: Lokaler Server (optional, z.B. fuer Live-Reload)
npx serve docs
```

---

## Tests

Die Unit-Tests koennen direkt im Browser ausgefuehrt werden:

```bash
open docs/tests.html
```

Getestet werden u.a.:
- Hilfsfunktionen (`getPieceType`, `getPieceColor`, `indexToAlgebraic`)
- Algebraische Notation
- Zugvalidierung (Bauer, Springer, Turm, Laeufer)
- Schach-Erkennung, Rochade, En Passant
- Undo, ungenuegendes Material, dreifache Stellungswiederholung

---

## Technologie-Stack

| Bereich     | Technologie           |
| ----------- | --------------------- |
| Sprache     | JavaScript (ES6+)     |
| Markup      | HTML5                 |
| Styling     | CSS3 (Custom Props)   |
| Schriftart  | Inter (Google Fonts)  |
| Figuren     | Unicode-Schachsymbole |
| Sound       | Web Audio API         |

---

## Arbeitsjournal

Das Arbeitsjournal mit woechentlichen Eintraegen befindet sich in der Datei [JOURNAL.md](JOURNAL.md).

---

## Autor

Entwickelt von **Seyedarvin Kasipourazbari** im Rahmen des Moduls 295 an der BBBaden.
