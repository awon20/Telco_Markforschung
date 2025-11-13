# Telco Marktforschung Workflow

## 1. Spreadsheet-Struktur finalisieren

Die Datei [`research_catalog_template.csv`](./research_catalog_template.csv) definiert die finale Struktur mit den Spalten **Quelle**, **Datum**, **Kategorie**, **Summary** und **Relevanz**. Verwende diese Datei als Vorlage in Google Sheets oder Excel und stelle sicher, dass alle Felder wie folgt gepflegt werden:

- **Quelle**: Name der Publikation, des Analysten oder der Datenbank.
- **Datum**: Veröffentlichungsdatum im ISO-Format (YYYY-MM-DD).
- **Kategorie**: Thematische Einordnung, z. B. „Marktanteile“, „AI-Initiativen“, „Wettbewerb“ oder „Regulierung“.
- **Summary**: Kurzfassung der wichtigsten Erkenntnisse (max. 2–3 Sätze).
- **Relevanz**: Qualitative Einschätzung (z. B. „Hoch“, „Mittel“, „Niedrig“).

## 2. Notion- oder Airtable-Datenbank anlegen und befüllen

1. **Neue Datenbank erstellen**
   - *Notion*: Neue Seite → „Table“ → „Full page“.
   - *Airtable*: Neues Base → „Start from scratch“ → „Grid view“.
2. **Spalten anlegen**
   - Name → „Quelle“ (Text).
   - Date → „Datum“ (Date field, ISO-Format aktivieren).
   - Select/Multiple select → „Kategorie“ (Optionen aus dem Spreadsheet übernehmen).
   - Long text → „Summary“.
   - Single select → „Relevanz“ (Optionen: Hoch, Mittel, Niedrig).
3. **Einträge importieren**
   - CSV-Import der Datei `research_catalog_template.csv`.
   - Nach dem Import Feldtypen prüfen und ggf. neu zuordnen.
4. **Tags vergeben**
   - Nutze zusätzliche Mehrfachauswahl-Felder, um Tags wie „Deutschland“, „5G“, „Kundenservice“ oder „Innovation“ zu vergeben.
   - Erstelle gespeicherte Filter oder Ansichten (z. B. „AI-Initiativen“ oder „Wettbewerb“).

## 3. Erste Visualisierungen in Data Studio oder Tableau

1. **Datenquelle verbinden**
   - Exportiere die Datenbank als CSV oder verbinde Data Studio/Tableau direkt mit Airtable.
2. **Visualisierungen vorbereiten**
   - **Marktanteile**: Balken- oder Kreisdiagramm nach Kategorie „Marktanteile“ mit Kennzahlen aus externen Quellen.
   - **AI-Initiativen**: Zeitstrahl oder Säulendiagramm nach Datum, gefiltert auf Kategorie „AI-Initiativen“.
3. **Dashboards aufbauen**
   - Erstelle getrennte Seiten/Tabs für Marktanteile und Innovationsinitiativen.
   - Ergänze Filter für Relevanz und Zeitraum, um die Analyse zu steuern.
4. **Nächste Schritte**
   - Ergänze Datenpunkte im Spreadsheet, synchronisiere die Datenquelle und erweitere das Dashboard um KPIs wie Kundenwachstum oder NPS, sobald Zahlen vorliegen.

## Wartung und Qualitätssicherung

- Aktualisiere das Spreadsheet wöchentlich und protokolliere neue Quellen in einer separaten Änderungs-Notiz.
- Führe quartalsweise einen Datenqualitäts-Check durch (Duplikate, veraltete Einträge).
- Dokumentiere größere Aktualisierungen und Visualisierungen in einem Changelog innerhalb von Notion oder Airtable.
