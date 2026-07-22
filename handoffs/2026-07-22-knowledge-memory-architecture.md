# Hand-off: Wissens- und Gedächtnisarchitektur

## Kontext
Martin möchte ein langfristiges Arbeitsgedächtnis für den Chief of Staff aufbauen, das rohe Gedanken aufnehmen, verdichten und in belastbares Wissen überführen kann.

## Entscheidungen
- Das System wird in drei Ebenen getrennt:
  1. **Inbox** für rohe, chronologische Dumps ohne Strukturzwang.
  2. **Chief of Staff / Middle Management** zur Verdichtung, Priorisierung und Ableitung von Aufgaben, Experimenten und Entscheidungen.
  3. **Executive Memory** als saubere, dauerhafte Wissensbasis.
- Martin arbeitet primär in der Inbox.
- Nur der Chief of Staff schreibt strukturiert ins Executive Memory.
- MCP ist eine Zugriffsschicht, kein Speicher.
- Obsidian ist primär Oberfläche und Editor, nicht die alleinige Wissensarchitektur.
- Ein Knowledge Graph soll explizite Beziehungen abbilden.
- Ein Vektorindex soll semantische Ähnlichkeit und freie Assoziation ermöglichen.
- Markdown/Git bleibt die portable Quelle der Wahrheit.

## Rollenverständnis
- Martin liefert Beobachtung, Intuition, Ideen und neue Konzepte.
- Der Chief of Staff übernimmt Verdichtung, Planung, Büroorganisation, zeitliche Einordnung und Priorisierung.
- Spezialagenten übernehmen Ausführung.

## Leitprinzipien
- Jede neue Information startet als **Inbox**, nicht als Wissen.
- Ideen, Annahmen, Entscheidungen, Experimente und Ergebnisse müssen getrennt behandelt werden.
- Das System soll Dopplungen, veraltete Inhalte und Widersprüche markieren.
- Das Ziel ist nicht maximale Speicherung, sondern bessere Entscheidungen und weniger Kontextwechsel.

## Offene Aufgaben
1. Datenmodell für das Executive Memory definieren.
2. Objekte festlegen, mindestens: Idee, Annahme, Entscheidung, Experiment, Ergebnis, Projekt, Person, Quelle.
3. Auswahl einer Graph-Datenbank prüfen.
4. Vektorindex festlegen.
5. MCP-Zugriff auf Git/Markdown, Graph und Vektorindex entwerfen.
6. Inbox-Kanäle definieren: Sprache, Instagram, Links, PDFs, Notizen.
7. Workflow bauen: Inbox → Verdichtung → Rückfrage → Executive Memory → Aufgaben/Agenten.
8. Regelmäßige Qualitätskontrolle für veraltete oder widersprüchliche Inhalte einführen.

## Nächster sinnvoller Schritt
Ein minimales Datenmodell und eine Ordnerstruktur definieren, bevor weitere Tools ausgewählt oder integriert werden.
