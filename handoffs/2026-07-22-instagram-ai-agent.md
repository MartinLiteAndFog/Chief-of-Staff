# Hand-off: Instagram-Wissensagent und Chief-of-Staff

**Datum:** 2026-07-22

## Kontext

Martin möchte gespeicherte und gelikte Instagram-Videos nicht mehr manuell aufarbeiten. Ein Agent soll Inhalte auswerten, Dubletten erkennen, Relevanz prüfen und daraus konkrete Handlungsempfehlungen für laufende Projekte ableiten.

## Entscheidungen

- Instagram soll künftig als Input-Kanal dienen, nicht als Wissensspeicher.
- Ein zentraler Chief-of-Staff-Agent soll Inputs, Projekte und ausführende Agenten koordinieren.
- Sprachgespräche in ChatGPT dienen als Denk- und Entscheidungsraum.
- Lokale bzw. ausführende Agenten wie Codex, Claude Code, n8n und Browser-Agenten übernehmen die Umsetzung.
- Nach relevanten Gesprächen wird per Befehl „Hand-off“ eine strukturierte Übergabe erzeugt und in diesem Repository gespeichert.

## Erkenntnisse

- Der Instagram-Export enthält Links, Captions und teils Transkripte, aber nicht immer die eigentlichen Videodateien.
- Ein großer Teil der gespeicherten KI-Inhalte wiederholt sich oder ist inzwischen veraltet.
- Der Agent soll daher nicht nur zusammenfassen, sondern bewerten:
  - Ist das neu?
  - Ist es noch aktuell?
  - Ist es belastbar oder nur Hype?
  - Für welches Projekt ist es relevant?
  - Welche konkrete Änderung der Arbeitsweise folgt daraus?
- Martins Stärke liegt bei Ideen, Aufmerksamkeit, Intuition und dem Aufspüren neuer Konzepte. Organisation, Verdichtung und Nachverfolgung sollen stärker ausgelagert werden.
- Vollautonomie ist ungeeignet. Der passende Modus ist ein Chief-of-Staff mit regelmäßiger Rückkopplung durch Martin.

## Aufgaben

### Priorität 1

- Zentrale Inbox definieren, in die Links, Exporte, PDFs und Gesprächs-Hand-offs eingehen.
- Einheitliches Datenformat für jeden Input festlegen:
  - Quelle
  - Kurzfassung
  - Kernaussagen
  - Neuheitsgrad
  - Aktualität
  - Vertrauensniveau
  - betroffene Projekte
  - Handlungsempfehlung
  - Duplikat-Verweise

### Priorität 2

- Einen ersten Workflow für Instagram-Reels testen:
  1. Link aus Export lesen
  2. Reel oder verfügbare Caption/Transkript abrufen
  3. Inhalt zusammenfassen
  4. gegen bestehendes Wissen prüfen
  5. Handlungsempfehlung erzeugen
  6. Ergebnis in der Wissensbasis speichern

- Chief-of-Staff-Briefing entwerfen:
  - drei neue relevante Erkenntnisse
  - zwei empfohlene Aktionen
  - eine Sache, die ignoriert werden sollte
  - offene Entscheidungen für Martin

### Priorität 3

- Projektbezogene Spezialagenten anbinden, zunächst für ein bis zwei Kernprojekte.
- Push-Mechanismus vorsehen, sobald ein neuer Hand-off im Repository landet.

## Offene Fragen

- Welche Wissensbasis soll zentral werden: Markdown/GitHub, Obsidian, Datenbank oder Kombination?
- Welcher lokale Agent überwacht dieses Repository?
- Wie soll der Push ausgelöst werden: GitHub Actions, n8n, lokaler Watcher oder Webhook?
- Welche Projekte werden zuerst angebunden?
- Wie viel Rohmaterial soll gespeichert werden, und wie viel nur als Verdichtung?

## Betroffene Projekte

- Chief-of-Staff-System
- Instagram-Wissensagent
- KI-Workflow-Orchestrierung
- mögliche spätere Quant-Strategieanalyse
- bestehende Projekte wie AllStreet

## Nächster sinnvoller Schritt

Einen minimalen Workflow bauen, der dieses Repository auf neue Dateien unter `handoffs/` überwacht und bei einem neuen Hand-off automatisch eine Aufgabe für den Chief-of-Staff-Agenten erzeugt.
