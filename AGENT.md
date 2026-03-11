# AGENT

## 1) Arbeitsprinzipien
- **Kleine PRs:** Änderungen in kleine, nachvollziehbare Pull Requests schneiden (ein klarer Zweck pro PR).
- **Keine geheimen Daten:** Keine Secrets, Zugangsdaten, Tokens oder personenbezogenen Daten im Repository ablegen.
- **Klare Commit-Messages:** Commit-Nachrichten präzise und handlungsorientiert formulieren (was/warum, nicht nur wie).

## 2) Strukturregeln
- **Neue Web-Dateien:** Neue Web-bezogene Dateien in die dafür vorgesehenen Web-Verzeichnisse legen (z. B. `web/`, `frontend/` oder vorhandene App-Struktur), nicht im Repo-Root verstreuen.
- **Legacy-Inhalte:** Bestehende Legacy-Artefakte klar getrennt in dedizierten Legacy-Ordnern ablegen (z. B. `legacy/`), inklusive kurzer Einordnung im jeweiligen Ordner.

## 3) Qualitäts-Gates
Vor Merge müssen mindestens folgende Gates erfolgreich sein:
- **Lint**
- **Format**
- **Build**
- **Link-Check** (für Doku/Markdown)

> Hinweis: Die konkreten Tools/Kommandos werden im nächsten Schritt je Technologie-Stack verbindlich festgelegt.

## 4) Dokumentationspflichten
Bei Strukturänderungen sind die zentralen Doku-Dateien mit zu aktualisieren:
- **README** (aktuelle Struktur, Einstieg, relevante Pfade)
- **PLAN** (Roadmap/Umsetzungsstand der Strukturmaßnahmen)

## 5) Definition of Done (DoD) für Struktur-Tasks
Ein Struktur-Task gilt als abgeschlossen, wenn:
- die Zielstruktur umgesetzt und nachvollziehbar ist,
- betroffene Pfade und Verantwortlichkeiten dokumentiert sind,
- README/PLAN aktualisiert wurden,
- alle definierten Qualitäts-Gates erfolgreich durchlaufen,
- keine offenen Migrations- oder Ablagefragen unbeantwortet bleiben.

## 6) Legacy/Talend: read-only oder migrieren?
**Policy (klar und verbindlich):**
- Legacy-/Talend-Inhalte sind standardmäßig **read-only**.
- Änderungen an Legacy/Talend erfolgen nur im Rahmen eines explizit geplanten Migrations-Tasks.
- Bei Migration gilt: schrittweise, nachvollziehbar, mit Mapping alt → neu und Rückverfolgbarkeit der Änderungen.
- Ohne freigegebenen Migrationsplan: **keine inhaltlichen Änderungen** an Legacy/Talend-Artefakten.
