# git-training-tmc

## Top-Level-Struktur

- `apps/` – Zielbereich für neue Web- und Applikationsentwicklung.
- `docs/` – Projektweite Dokumentation und Migrationsentscheidungen.
- `legacy/` – Bestehende Altsysteme, die getrennt weitergeführt oder archiviert werden.

## Warum die Trennung?

Die bisherige Talend-Struktur (`TMC_GIT/`) wurde nach `legacy/talend/TMC_GIT/` verschoben, um Legacy-Artefakte klar von neuer Entwicklung zu isolieren. So werden folgende Ziele erreicht:

1. **Klare Verantwortlichkeiten**: Legacy-Wartung und Neuentwicklung laufen in getrennten Bereichen.
2. **Weniger Risiko für neue Features**: Web-Entwicklung landet nicht mehr versehentlich in Talend-Verzeichnissen.
3. **Bessere Archivierbarkeit**: Generierte Talend-Dateien können gezielt ignoriert/ausgelagert werden.

## Guardrail für neue Entwicklung

Neue Web-Projekte, Frontends und zugehörige Tooling-Dateien gehören ausschließlich in `apps/` (plus ggf. `docs/` für Doku) und **nicht** in `legacy/`.
