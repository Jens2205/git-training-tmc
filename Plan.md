# Strukturmigrationsplan

## Entscheidung

Das Talend-Projekt wurde in einen dedizierten Legacy-Baum verschoben: `legacy/talend/TMC_GIT/`.

## Begründung der Trennung

- **Technische Entkopplung**: Legacy-Talend-Artefakte und neue Web-/App-Entwicklung haben unterschiedliche Build-, Runtime- und Release-Zyklen.
- **Team-Fokus**: Klare Bereiche erleichtern Ownership und reduzieren Konflikte im Tagesgeschäft.
- **Sauberer Projektaufbau**: Top-Level-Struktur (`apps/`, `docs/`, `legacy/`) ist langfristig verständlich und skalierbar.
- **Option auf Auslagerung**: Der Legacy-Baum kann bei produktiver Relevanz später in ein eigenes Repository überführt werden.

## Leitlinie für künftige Änderungen

- Neue Web-Entwicklung wird ausschließlich unter `apps/` umgesetzt.
- Änderungen unter `legacy/` sind auf Wartung, Stabilisierung und Migration beschränkt.
- Generierte Talend-Artefakte werden über `.gitignore` gesteuert und bei Bedarf archiviert.
