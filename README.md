# BLOCKOUT - 3D Pit

BLOCKOUT ist eine browserbasierte 3D-Variante eines Tetris-artigen Geschicklichkeitsspiels. Mehrere geometrische Formen fallen in einen dreidimensionalen Schacht. Ziel ist es, vollständige Schichten zu bilden und zu entfernen.

Das Spiel wird vollständig als einzelne HTML-Datei umgesetzt und benötigt keine Installation von Paketen oder Build-Schritten.

## Funktionen

- Dreidimensionale Darstellung des Spielschachts
- Mehrere Schachtgrößen
- Verschiedene 3D-Spielfiguren
- Rotation auf drei Achsen
- Soft Drop und Hard Drop
- Punktestand, Level, entfernte Schichten und gesetzte Blöcke
- Pause-Modus
- Optionaler 8-Bit-Sound mit Hintergrundmelodie und Spieleffekten
- Responsive Darstellung für Desktop und mobile Bildschirmgrößen

## Schachtgrößen

- `3 × 3 × 10`
- `5 × 5 × 10` - Standard
- `5 × 5 × 12`

Der Wechsel der Schachtgröße startet bei laufendem Spiel automatisch ein neues Spiel.

## Starten

1. Das Repository herunterladen oder klonen.
2. Die Datei `blockout.html` in einem aktuellen Browser öffnen.

Alternativ kann der Ordner mit einem lokalen Webserver bereitgestellt werden, zum Beispiel mit Python:

```powershell
python -m http.server 8000
```

Danach im Browser `http://localhost:8000/blockout.html` aufrufen.

## Steuerung

| Taste | Aktion |
| --- | --- |
| Pfeiltaste links/rechts | Bewegung auf der X-Achse |
| Pfeiltaste hoch/runter | Bewegung auf der Y-Achse |
| `Q` / `E` | Rotation um die X-Achse |
| `W` / `S` | Rotation um die Y-Achse |
| `A` / `D` | Rotation um die Z-Achse |
| `Shift` / `C` | Stein eine Ebene weich fallen lassen |
| `Leertaste` | Stein sofort fallen lassen |
| `P` | Spiel pausieren/fortsetzen |
| `R` | Neues Spiel starten |
| `Enter` | Spiel starten |

Der Button **NEUES SPIEL** startet das Spiel ebenfalls neu. Über **SOUND: AN/AUS** kann die Audiowiedergabe aktiviert oder deaktiviert werden.

## Wertung

- Soft Drop bringt zusätzliche Punkte.
- Hard Drop bringt für jede zurückgelegte Ebene zusätzliche Punkte.
- Das Entfernen vollständiger Schichten bringt Bonuspunkte.
- Das Level steigt alle fünf entfernten Schichten.
- Mit höherem Level fallen die Steine schneller.

## Technologie

- HTML5
- CSS
- JavaScript
- Canvas 2D API
- Web Audio API

## Browser

Für alle Funktionen wird ein aktueller Browser mit aktivierter JavaScript-Ausführung benötigt. Die Web Audio API wird für den Sound verwendet.
