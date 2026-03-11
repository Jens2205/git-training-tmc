# Legacy-Archivhinweise (Talend)

Der Ordner `legacy/talend/TMC_GIT/` enthält ein bestehendes Talend-Projekt.

## Was nicht ins Git-Repo gehört

- Generierte Build-Ausgaben (z. B. `target/`, lokale `src/`-Generierung).
- Temporäre Arbeitsverzeichnisse (`temp/`).
- Laufzeit- und Tooling-Logs (`*.log`).
- IDE-/Workspace-Dateien (`.classpath`, `.project`, Backup-Dateien).

## Empfehlung für produktive Relevanz

Falls das Talend-Projekt weiterhin produktiv betrieben wird, sollte mittelfristig eine Auslagerung in ein eigenes Repository geprüft werden (inkl. eigener CI/CD- und Release-Strategie).
