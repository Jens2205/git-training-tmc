# Plan.md – Roadmap (lebendes Dokument)

## Zielbild
Aus dem aktuellen Repository einen klar strukturierten Ausgangspunkt für eine moderne Website zur Reflexintegration machen.

## Phase 1 – Struktur klären (in Arbeit)
- [x] Steuerdokumente anlegen (`README.md`, `AGENT.md`, `Plan.md`)
- [ ] Zielordner real anlegen (`apps/`, `content/`, `docs/`, `legacy/`)
- [ ] Legacy-Pfad für Talend festlegen und dokumentieren

## Phase 2 – Legacy sauber abtrennen
- [ ] `TMC_GIT/` nach `legacy/talend/TMC_GIT/` verschieben
- [ ] Verweise/Erklärungen in README aktualisieren
- [ ] Optional: Entscheidung treffen, ob Talend-Bestand in eigenes Archiv-Repo wandert

## Phase 3 – Web-Fundament setzen
- [ ] Ziel-Stack auswählen (Next.js/Astro/anderer)
- [ ] Basisprojekt unter `apps/web/` initialisieren
- [ ] Erste Seitenstruktur definieren (Start, Angebot, Über uns, Kontakt)

## Phase 4 – Content- und Betriebsreife vorbereiten
- [ ] Inhaltsmodelle für Leistungen/Themen/Kontakt in `content/` festlegen
- [ ] Architektur- und Redaktionsleitfäden in `docs/` ergänzen
- [ ] Qualitätschecks (Format/Lint/Build) einführen

## Risiken / offene Entscheidungen
- Welcher Web-Stack passt langfristig am besten?
- Soll Legacy nur archiviert oder vollständig ausgelagert werden?
- Welche Kontaktform (Formular/Telefon/E-Mail) ist rechtlich und organisatorisch sinnvoll?

## Änderungslog
- 2026-03-11: Initiale Roadmap erstellt.
