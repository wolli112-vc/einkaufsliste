# Einkaufsliste

Einfache Einkaufsliste als Home Assistant Add-on.

## Funktionen

- **Anzahl**: Mengensteuerung per +/- Buttons
- **Kategorie**: Frei eingebare Kategorien mit Vorschlägen
- **Produkt**: Produkte nach Kategorie gruppiert
- **Suche**: Filter über Produkt und Kategorie
- **Löschen**: Einzelne Einträge oder alle auf einmal entfernen
- **Persistent**: Daten werden unter `/share/einkaufsliste/` gespeichert

## Installation

1. Füge dieses Repository zu Home Assistant hinzu
2. Installiere das Add-on "Einkaufsliste"
3. Starte das Add-on
4. Öffne die Weboberfläche über das Seitenpanel

## API

- `GET /api/items` – Alle Einträge
- `POST /api/items` – Neuen Eintrag hinzufügen
- `PUT /api/items/<id>` – Eintrag aktualisieren
- `DELETE /api/items/<id>` – Eintrag löschen
- `POST /api/clear` – Alle Einträge löschen
- `GET /api/categories` – Alle Kategorien
