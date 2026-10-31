# VeniceRadio FS – Änderungen 0.4.5-R3 → 0.4.5-R4

**Quellstand 31. Oktober 2026.** Die R4-Änderungen sind im Quellcode integriert und durch Java-Regressionstests geprüft. Die praktische Abnahme an unterschiedlichen Geräten läuft noch.

## Bedienoberfläche

- Kachelradius und Radius der unteren Navigation zentral auf **12 dp** vereinheitlicht; Suchfeld/kleinere Schaltflächen bleiben separat bei **9 dp**.
- Abstände, Haarlinien, Kachelunterkanten und zweizeilige Beschriftungen vereinheitlicht; Ladekreis links in der Statuszeile.
- Korrekturen beim Wechsel der Favoriten-Unteransichten, damit keine transparenten oder abweichenden Kartenstile zurückbleiben.
- **Noch nicht Bestandteil:** neue responsive Displayanordnung – das ist Planung für 0.4.6.

## Verlauf und Identität

- „Zuletzt gehört“ getrennt für jedes eindeutig erkannte Radio, höchstens sechs Einträge.
- Internetradio, DAB und UKW sowie unterscheidbare Regional-/Verzeichniseinträge bleiben getrennt, auch bei ähnlichen oder identischen Namen.
- Alte Verlaufseinträge ohne gesicherte Gerätezuordnung werden nicht angezeigt; bestehende Favoriten und Ordner sollen erhalten bleiben.
- Gespeicherte Routen werden nur im bestätigten passenden Empfangsmodus geöffnet; mehrdeutige Sender werden nicht willkürlich ausgewählt.
- Ein verkürzter Wiedergabename erzeugt keinen nicht abspielbaren Phantom-Verlaufseintrag mehr. Ein ausschließlich direkt am Radio erstmals gewählter Sender erscheint daher möglicherweise nicht sofort im App-Verlauf.

## Diagnose, Stabilität und Sicherheit

- Rein lesende WLAN-Scanliste mit bis zu 200 Einträgen, maximal acht Abfragen und 15-Sekunden-Budget; Teilresultate bei Abbruch gekennzeichnet.
- Verbesserte parallele Datenverarbeitung bei Verlauf, Favoriten und Entdecken.
- Schutz bei unbestätigter Radiospeicherung: erst nachlesen, danach gegebenenfalls erneute Auswahl durch den Benutzer; kein blindes Wiederholen.

## Wartbarkeit und Kompatibilität

- Nicht mehr benötigte Codeelemente entfernt, Designwerte zentralisiert.
- Java-Paket auf `org.veniceradio.fs` umbenannt; Anwendungskennung gleich geblieben, bisherige Launcher-Komponente wird als Alias bereitgestellt.
- R4-Quellstand: `versionCode 57`, `versionName 0.4.5-R4`.
- Laut Entwicklungsprotokoll **37/37 Java-Workflow-Schritte** bestanden, plus Stub-Kompilierung. **Die praktische Geräteprüfung für R4 steht noch aus.**

## Nicht in R4 eingeflossen

- Responsive Smartphone-Umgestaltung, Tablet-/Querformat und Mehrsprachigkeit: [0.4.6](ROADMAP-0.4.6.md).
- Neue DLNA-Pause-/Skip-Tasten: [R5](ROADMAP-R5.md).

Detaillierte Entwicklungsprotokolle, interne Testergebnisse und technische Arbeitsstände verbleiben in der **privaten** Entwicklungsumgebung.
