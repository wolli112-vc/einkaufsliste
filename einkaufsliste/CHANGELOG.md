# Changelog

## 1.0.8 – 2026-07-17
- **File-Locking** hinzugefügt: Alle Dateizugriffe (`load_data` + `save_data`) nutzen jetzt `fcntl`-Locks, um gleichzeitige Schreibzugriffe zu verhindern
- Das ist Voraussetzung für die Integration mit der Warenwirtschaft, die jetzt direkt in die Einkaufsliste schreiben kann

## 1.0.7 – 2026-07-13
- Spaltenreihenfolge angepasst: Anzahl, Produkt, Kategorie (Kategorie steht jetzt am Ende)

## 1.0.6 – 2026-07-13
- Liste aktualisiert sich jetzt automatisch alle 10 Sekunden (zusätzlich zum manuellen 🔄-Button)
- Auto-Update pausiert automatisch, während ein Eintrag inline bearbeitet wird

## 1.0.5 – 2026-07-13
- 🔄 Aktualisieren-Button hinzugefügt, um die Liste manuell neu zu laden
- Einträge können jetzt per Klick inline bearbeitet werden (Anzahl, Kategorie, Produkt)

## 1.0.4 – 2026-07-13
- `repository.yaml`: Name auf "wolli112-vc Addon Repo" geändert, damit alle Add-ons im HA Store unter demselben Repository-Namen erscheinen

## 1.0.3 – 2026-07-13
- Neues Produkt kann jetzt zusätzlich zum Button auch mit der Enter-Taste hinzugefügt werden

## 1.0.2 – 2026-07-13
- Einzelnes Löschen per ✕ erfolgt jetzt ohne Bestätigungsdialog (direkt)
- Bestätigungsdialog bleibt nur bei "Alles löschen" erhalten

## 1.0.1 – 2026-07-13
- Löschen-Button (✕) von der rechten Seite direkt neben +/− in die Buttons-Spalte verschoben
- Gleiche Button-Optik: roter Kreis mit weißem ✕ wie bei −
- Spaltenanzahl reduziert (keine separate Aktionsspalte mehr)

## 1.0.0 – 2026-07-13
- Erstveröffentlichung des Add-Ons "Einkaufsliste"
- Verwaltung von Einkaufsartikeln mit Anzahl, Kategorie und Produkt
- Gruppierung nach Kategorie mit visuellen Headern
- Frei eingebare Kategorien mit Vorschlägen aus bestehenden Einträgen
- Mengensteuerung per `+`/`-` Buttons
- Direktes Löschen einzelner Einträge
- Funktion zum Löschen aller Einträge
- Suchfunktion über Produkt und Kategorie
- Persistente Datenhaltung unter `/share/einkaufsliste/einkaufsliste.json`
- Ingress-Support für Home Assistant Integration
- Responsive Design für Mobile und Desktop
