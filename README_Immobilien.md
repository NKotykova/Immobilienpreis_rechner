# Immobilienpreis-Rechner – Deutschland

Grafische Anwendung zur Schätzung des Immobilienwertes in Deutschland auf Basis von 10 Eingabeparametern.

## Funktionsweise

Der Benutzer gibt Grundstücksfläche, Wohnfläche und Baujahr ein und wählt aus Dropdown-Menüs: Bundesland, Lage (Stadt/Land), Hausart, Ausstattung, Architektenhaus, Makler und Denkmalschutz. Das Ergebnis wird sofort als geschätzter Preis in Euro angezeigt.

## Berechnungslogik

Basis: Grundstück × 160 €/m² + Wohnfläche × 2.500 €/m² − Altersabschlag (0,1 € pro Jahr).
Anschließend werden Faktoren aus `datei.json` multipliziert (z.B. Hamburg × 2,5, Sachsen-Anhalt × 0,6).

## Dateien

| Datei | Beschreibung |
|---|---|
| `Immobilienpreis_rechner.ipynb` | Hauptprogramm mit GUI |
| `datei.json` | Preisfaktoren nach Bundesland, Hausart, Ausstattung u.a. |

## Voraussetzungen

Python 3.x, Standardbibliotheken: `tkinter`, `json`, `datetime`

## Starten

```bash
jupyter notebook Immobilienpreis_rechner.ipynb
```

## Autorin

Nadiia Kotykova
