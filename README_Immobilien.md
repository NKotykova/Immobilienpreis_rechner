# Immobilienpreis-Rechner – Deutschland

Grafische Anwendung zur Schätzung des Immobilienwertes in Deutschland auf Basis von 10 Eingabeparametern.

## Funktionsweise

Der Benutzer gibt Grundstücksfläche, Wohnfläche und Baujahr ein und wählt aus Dropdown-Menüs: Bundesland, Lage (Stadt/Land), Hausart, Ausstattung, Architektenhaus, Makler und Denkmalschutz. Der geschätzte Preis wird sofort in Euro angezeigt.

## Berechnungsformel

```
Basispreis = Grundstück × 160 €/m² + Wohnfläche × 2.500 €/m² − Altersabschlag
Gesamtpreis = Basispreis × Faktor(Bundesland) × Faktor(Ort) × ... (aus datei.json)
```

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
