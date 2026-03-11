# Reflexintegration Website – Projekt-README

Dieses Repository wird von einem alten Talend-Projektstand auf eine moderne, wartbare Webprojekt-Struktur umgestellt.

## Ziel
Eine freundliche, vertrauensvolle Website für das Angebot zur Reflexintegration mit:
- klaren Informationen zum Thema
- Übersicht der Leistungen/Angebote
- einfacher Kontaktmöglichkeit

## Aktueller Stand (Ist)
- Es existiert überwiegend ein historischer Talend-Bestand unter `TMC_GIT/`.
- Eine moderne Web-App-Struktur ist noch nicht aufgebaut.

## Zielstruktur (Soll)
Die folgende Struktur ist der nächste sinnvolle Schritt für den Umbau:

```text
.
├─ apps/
│  └─ web/                  # spätere Website (z. B. Next.js/Astro/Vite)
├─ content/
│  ├─ angebote/
│  ├─ themen/
│  └─ kontakt/
├─ docs/
│  ├─ architecture.md
│  ├─ content-guidelines.md
│  └─ decisions/
├─ legacy/
│  └─ talend/
│     └─ TMC_GIT/           # historischer Bestand (schrittweise entkoppeln)
├─ AGENT.md                 # lebende Arbeitsregeln
├─ Plan.md                  # lebende Roadmap
└─ README.md
```

## Migrationsprinzip
1. **Nicht mischen:** Neue Webentwicklung nicht im Legacy-Bereich starten.
2. **Dokumentieren:** Jede Strukturentscheidung in `Plan.md` und `docs/decisions/` festhalten.
3. **Kleine Schritte:** In kleinen Commits umbauen, damit Änderungen nachvollziehbar bleiben.

## Nächster geplanter Umsetzungsschritt
- Ordnerstruktur gemäß „Zielstruktur“ erstellen
- Talend-Bestand nach `legacy/talend/` verschieben
- Web-Stack-Entscheidung treffen (z. B. Next.js vs. Astro)
- Basis-App unter `apps/web/` initialisieren

## Hinweise für Mitarbeit
- Arbeitsregeln: `AGENT.md`
- Umsetzungspfad: `Plan.md`
