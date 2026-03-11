# Projektübersicht: Website Reflexintegration

## 1. Kurzbeschreibung
Dieses Repository dient als Grundlage für den Aufbau einer Website zum Thema **Reflexintegration**. Ziel ist eine klar strukturierte, wartbare und erweiterbare Projektbasis für den Webauftritt.

### Ziel der Website
- Information über Angebote und Leistungen im Bereich Reflexintegration bereitstellen.
- Vertrauen durch klare Inhalte, transparente Struktur und einfache Kontaktwege schaffen.
- Eine technische Basis schaffen, die spätere Erweiterungen (z. B. Blog, Terminbuchung, Mehrsprachigkeit) ermöglicht.

### Zielgruppe
- Eltern von Kindern mit Entwicklungs- oder Lernauffälligkeiten.
- Erwachsene mit Interesse an Reflexintegration.
- Pädagogische und therapeutische Fachpersonen.

### Primäre Nutzeraktionen
- Kontakt aufnehmen (Formular, E-Mail, Telefon).
- Angebote/Leistungen verstehen.
- Hintergrundinformationen lesen.
- Optional: Termin- oder Erstgespräch anfragen.

---

## 2. Aktueller Ist-Zustand
Der aktuelle Stand des Repositories ist technisch gemischt:

- Es sind **Talend-Artefakte** vorhanden.
- Ein moderner, klar erkennbarer **Web-Stack** (z. B. Frontend-App mit Build-/Run-Setup) ist derzeit nicht oder nicht konsistent sichtbar.
- Die aktuelle Struktur erschwert die direkte Weiterentwicklung zu einem sauberen Webprojekt.

Konsequenz: Für eine nachhaltige Weiterentwicklung ist eine klare Zielstruktur mit Trennung von Altbestand und neuem Webprojekt sinnvoll.

---

## 3. Zielstruktur des Repositories
Empfohlene Zielstruktur:

```text
.
├─ apps/
│  └─ web/               # Haupt-Webanwendung (finaler Stack wird noch entschieden)
├─ content/              # Inhalte (Texte, Bilder-Metadaten, ggf. CMS-Export)
├─ docs/                 # Projektdokumentation, Architektur, Entscheidungen
├─ infra/                # Deployment, Hosting, CI/CD, IaC-Skripte
├─ legacy/
│  └─ talend/            # Übernommene Talend-Artefakte (nur Altbestand)
└─ README.md
```

### Strukturprinzipien
- **Trennung von Neu und Alt**: Aktive Webentwicklung in `apps/web`, historische Artefakte in `legacy/talend`.
- **Dokumentation nah am Code**: Technische und fachliche Entscheidungen in `docs/`.
- **Inhalte entkoppeln**: Wiederverwendbare Inhalte in `content/`, unabhängig von Implementierungsdetails.
- **Betrieb explizit abbilden**: Infrastrukturthemen zentral unter `infra/`.

---

## 4. Quickstart für lokale Entwicklung
> Hinweis: Der finale Web-Stack ist noch nicht entschieden. Die folgenden Schritte sind bewusst als Platzhalter angelegt.

### Voraussetzungen (Platzhalter)
- Laufzeitumgebung gemäß finaler Stack-Entscheidung
- Paketmanager gemäß finaler Stack-Entscheidung
- Optional: Container-Laufzeit für lokale Infrastruktur

### Geplanter Ablauf
1. Repository klonen.
2. Abhängigkeiten für `apps/web` installieren.
3. Entwicklungsserver starten.
4. Lokale URL im Browser öffnen.

### Platzhalter-Kommandos
```bash
# 1) Repository klonen
git clone <repo-url>
cd git-training-tmc

# 2) Abhängigkeiten installieren (final abhängig vom Stack)
<package-manager> install

# 3) Entwicklungsserver starten
<package-manager> run dev
```

Nach finaler Stack-Entscheidung wird dieser Abschnitt mit konkreten, lauffähigen Befehlen aktualisiert.

---

## 5. Entscheidungslog
Warum diese Struktur gewählt wurde:

1. **Wartbarkeit**
   - Klare Modulgrenzen erleichtern Onboarding, Betrieb und Weiterentwicklung.
2. **Migrationsfähigkeit**
   - Altbestand bleibt nachvollziehbar erhalten, ohne die neue Webentwicklung zu blockieren.
3. **Skalierbarkeit**
   - Die Struktur unterstützt zukünftige Erweiterungen (weitere Apps, CMS-Anbindung, Automatisierung).
4. **Teamfähigkeit**
   - Unterschiedliche Rollen (Content, Entwicklung, Ops) können parallel arbeiten.
5. **Risikominimierung**
   - Historische Artefakte werden konserviert statt ad hoc gelöscht.

---

## 6. Migration von Altbestand
Ziel der Migration ist die kontrollierte Überführung relevanter Inhalte aus dem Altbestand in die neue Struktur.

### Umgang mit `TMC_GIT/`
- `TMC_GIT/` wird als **Bestandsquelle** betrachtet, nicht als Ziel für neue Entwicklung.
- Relevante Artefakte werden gesichtet, klassifiziert und bei Bedarf nach `legacy/talend/` überführt.
- Neue Features und aktiver Webcode entstehen ausschließlich in der Zielstruktur (insb. `apps/web`).

### Empfohlenes Vorgehen
1. **Inventarisierung**
   - Inhalte in `TMC_GIT/` erfassen (Dateitypen, Relevanz, Abhängigkeiten).
2. **Klassifizierung**
   - Behalten (historisch), migrieren (fachlich relevant), verwerfen (obsolet).
3. **Überführung**
   - Historische Talend-Artefakte nach `legacy/talend/` verschieben oder spiegeln.
4. **Dokumentation**
   - Entscheidungen und Begründungen in `docs/` festhalten.
5. **Abschluss**
   - Nachvollziehbare Zuordnung: Was wurde übernommen, was bleibt archiviert, was entfällt.

### Migrationsprinzipien
- Keine unkommentierte Löschung von Altmaterial.
- Jede strukturelle Änderung dokumentieren.
- Fachlich relevante Inhalte priorisiert in die neue Webstruktur überführen.

---

## Nächste Schritte
- Finalen Web-Stack entscheiden (z. B. Framework, Build-Tool, Hosting-Strategie).
- Ordnerstruktur gemäß Zielbild initial anlegen.
- Migrationsinventur für `TMC_GIT/` starten und dokumentieren.
