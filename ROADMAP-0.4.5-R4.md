# VeniceRadio FS 0.4.5-R4 – Implementiert und noch zu prüfen

**Stand 31. Oktober 2026.** Diese Seite trennt den implementierten R4-Quellstand von noch ausstehenden Geräteprüfungen. Die Entwicklung läuft derzeit in kleinem privatem Rahmen.

## Im R4-Quellstand umgesetzt

- [x] Einheitliche Designregeln: 12-dp-Kartenradius und Navigationsradius, zentrale Kachelabstände, konsistente Grundlinien, zweizeilige Beschriftungen und Ladezustände
- [x] Geräterichtige Historie mit maximal sechs „Zuletzt gehört“-Sendern pro bestätigtem Radio; sichere Behandlung alter nicht zuordenbarer Verlaufseinträge
- [x] Trennung nach Empfangsmodus und Sender-/Verzeichnisidentität, ohne Namensnormalisierung oder blindes Auswählen des ersten gleichnamigen Senders
- [x] Prüfung des tatsächlichen Empfangsmodus vor Wiederaufruf gespeicherter Sender
- [x] Thread-Schutz bei Favoriten, Verlauf sowie den Ansichtslisten für Entdecken
- [x] Lesendes WLAN-Paging mit maximal acht Abfragen, höchstens 200 Einträgen, Zeitbudget und Kennzeichnung unvollständiger Resultate
- [x] Sicherer Wiederanlauf nach nicht bestätigtem Radiospeichervorgang: Zustand zuerst lesen, keine automatische zweite Schreibaktion
- [x] Bereinigung nicht referenzierter Codeelemente und Umzug des Java-Pakets auf `org.veniceradio.fs`; alter Launcher-Komponentenname bleibt als Kompatibilitätsalias
- [x] Dokumentierte Java-Workflow-Prüfungen: **37 von 37 bestanden**, ergänzende Regressionstests vorhanden

## Für die R4-Freigabe noch offen

- [ ] R4-Änderungen auf tatsächlich vorhandenen Radios und Smartphones überprüfen, einschließlich Übernahme bestehender Favoriten und Verlaufsdaten
- [ ] Sichttest und Bediengeschwindigkeit auf realen Telefonen überprüfen, einschließlich der zweizeiligen langen Sendernamen und der Kachelgrundlinien
- [ ] WLAN-Feldnamen und tatsächliche unterstützte FSAPI-Knoten an verschiedenen Radios bestätigen
- [ ] DAB/UKW-Menüs und Senderidentitäten an echten Geräten überprüfen
- [ ] B5: Preset-Name und Wiedergabename anhand echter Geräteantworten abgleichen, ohne unbestätigte Schreibtests
- [ ] Gestaltung gleichnamiger Senderkacheln über unterschiedliche Modi entscheiden, ohne zusätzliche Textzeile
- [ ] Entscheidungen zu den bisher nicht freigegebenen DAB/UKW-Icons gesondert treffen

**Keine Hersteller-Workarounds:** Maßstab bleibt das von der Firmware tatsächlich angebotene FSAPI-Verhalten.

Siehe [Änderungen R3 → R4](AENDERUNGEN-0.4.5-R3-ZU-R4.md), [FAQ](FAQ.md), [0.4.6](ROADMAP-0.4.6.md) und [R5](ROADMAP-R5.md).
