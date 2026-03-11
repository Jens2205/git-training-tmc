# Plan

## 1. Phasenmodell

### Phase 1: Audit
- Bestandsaufnahme der aktuellen Codebasis, Infrastruktur, Build-/Deploy-Prozesse und Inhalte.
- Identifikation von Altlasten, Doppelstrukturen und fehlender Dokumentation.
- Erfassung technischer Schulden und Quick Wins.

### Phase 2: Zielstruktur
- Definition der Zielarchitektur (Code-Struktur, Tooling, Deployment, Betriebsmodell).
- Festlegung von Standards für Ordnerstruktur, Naming, Qualitätssicherung und Dokumentation.
- Abstimmung der Zielstruktur mit Stakeholdern inkl. Go/No-Go-Entscheid.

### Phase 3: Migration
- Umsetzung der Zielstruktur in priorisierten Migrationswellen.
- Schrittweise Überführung von Modulen/Features inkl. Tests und Übergabe.
- Parallelbetrieb nur dort, wo zur Risikominimierung erforderlich.

### Phase 4: Aufräumen
- Entfernen nicht mehr benötigter Altdateien, Konfigurationen und Abhängigkeiten.
- Konsolidierung der Dokumentation, Runbooks und Betriebsprozesse.
- Abschlussreview und formale Abnahme.

## 2. Konkrete Arbeitspakete

| Reihenfolge | Arbeitspaket | Verantwortlichkeit | Abnahmekriterium |
|---|---|---|---|
| 1 | Repository- und Infrastruktur-Audit durchführen (Code, Deploy, Abhängigkeiten) | Tech Lead + DevOps | Audit-Report liegt vor, inkl. Liste kritischer Findings |
| 2 | Ziel-Stack und Zielarchitektur verbindlich festlegen | Architektur-Team + Product Owner | Architektur-Entscheid dokumentiert und von Stakeholdern freigegeben |
| 3 | Ziel-Ordnerstruktur und Coding-Standards definieren | Tech Lead + Senior Devs | Struktur-/Style-Guide veröffentlicht, Team-Review abgeschlossen |
| 4 | Migrationsplan in Wellen aufteilen (Scope, Aufwand, Reihenfolge) | Projektleitung + Tech Lead | Abgestimmter Migrationsfahrplan mit Terminen vorhanden |
| 5 | Pilot-Migration eines abgegrenzten Moduls durchführen | Umsetzungsteam | Modul läuft in Zielstruktur, Tests grün, keine Blocker offen |
| 6 | Hauptmigration gemäß Wellenplan umsetzen | Umsetzungsteam | Alle priorisierten Module migriert und integriert |
| 7 | Altdateien, Legacy-Configs und ungenutzte Artefakte entfernen | Umsetzungsteam + DevOps | Bereinigungsliste vollständig abgearbeitet, Build/Deploy stabil |
| 8 | Dokumentation, Betriebsübergabe und Abschlussabnahme | Tech Lead + Betrieb + Product Owner | Betriebsdoku aktuell, Übergabe erfolgt, Abnahmeprotokoll unterzeichnet |

## 3. Risiken / Abhängigkeiten

- **Unklarer Ziel-Stack:** Verzögert Architekturentscheidungen und erzeugt Rework.
- **Altdateien ohne klaren Nutzen:** Risiko unbeabsichtigter Löschungen oder toter Pfade.
- **Fehlende Testabdeckung:** Erhöht Regressionen während der Migration.
- **Abhängigkeit von Schlüsselpersonen:** Wissensinseln können Fortschritt blockieren.
- **Zeitliche Abhängigkeit zu laufenden Features:** Parallelentwicklung kann Merge-Konflikte verstärken.
- **Betriebliche Randbedingungen:** CI/CD, Hosting oder Security-Vorgaben können Zielbild einschränken.

## 4. Backlog „später“

- Design-System aufbauen und in Komponentenbibliothek überführen.
- CMS-Einbindung evaluieren und ggf. einführen.
- Mehrsprachigkeit (i18n/l10n) konzeptionieren und umsetzen.
- SEO-Basics und technisches SEO (Metadaten, Performance, Struktur) systematisch ausbauen.

## 5. Change-Log

| Datum | Änderung | Grund |
|---|---|---|
| 2026-03-11 | Initiale Version des Plans erstellt (Phasenmodell, Arbeitspakete, Risiken, Backlog, Change-Log). | Startpunkt für ein lebendes Planungsdokument schaffen. |

