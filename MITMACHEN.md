# Mitmachen: VeniceRadio FS auf unterschiedlichen Radios testen

**Testaufruf – Stand 31. Oktober 2026.** VeniceRadio FS richtet sich an Besitzer kompatibler FSAPI-Internetradios, gerade auch älterer Geräte. Ziel ist, die Unterstützung **über Protokollfähigkeiten statt über Hersteller-Sonderwege** abzusichern.

## Besonders hilfreiche Tests

1. **Geräteverbindung:** Modell, Firmwarestand, vom Radio angebotene FSAPI-Quellen und Stabilität beim Wiederverbinden.
2. **Entdecken und Favoriten:** verschachtelte Verzeichnisse, Suchergebnisse, Senderlogos, Zurück-Navigation und Favoritenordner.
3. **„Zuletzt gehört“:** Wechsel zwischen zwei Radios; identische Namen bei Internet/DAB/UKW; regionale Varianten und Einträge mit Zusätzen wie „laut.fm“.
4. **WLAN-Diagnose:** nur lesende Informationen, Scanlisten auch über 25 Einträge, Hinweise bei fehlenden oder unvollständigen Werten.
5. **Oberfläche:** Kachelgrundlinien, zweizeilige Namen, Seitenbedienung und Performance auf unterschiedlichen Smartphone-Größen.
6. **Radiospeicher:** vorerst **nur auslesen und vorhandene belegte Plätze vergleichen**. Kein unbeaufsichtigtes Überschreiben und keine Suchläufe.

## Wichtig für die Testphase

- R4 ist nach den bisherigen Quellcode-Prüfungen **noch kein bestätigter öffentlicher APK-Release**. Testpakete werden nur über die ausdrücklich angegebenen Projektkanäle verteilt; in diesem Repository gibt es keinen APK-Download.
- Keine Werksresets, DAB-Suchläufe, WLAN-Änderungen oder Schreibtests an Radiospeichern ohne gesonderte Freigabe.
- Bitte bei einem Fehler angeben: Gerätemodell, Firmware, Android-Version, App-Version, genauer Bedienweg, erwartetes und tatsächliches Ergebnis.
- Screenshots des Diagnoseprotokolls können helfen, aber **PIN, Session-ID, private IP, WLAN-Namen und BSSID** vorher schwärzen oder ausreichend kürzen.
- Die drei Voraussetzungen für freigegebene öffentliche App-Screenshots bleiben: zentrierte Piktogramme, korrekte Favoriten-/Ordnernavigation und funktionierende DLNA-Navigation mit Coverdarstellung.

## Was bereits feststeht

Die Entwicklung nutzt eine gemeinsame FSAPI-Implementierung. Unterschiedliche Geräte können unterschiedliche Knoten und Menüs anbieten; daraus wird kein Hersteller-Sonderfall abgeleitet. Rückmeldungen sollen helfen, das reale Protokollverhalten zu dokumentieren.

Siehe auch [FAQ](FAQ.md), [R4-Status](ROADMAP-0.4.5-R4.md) und [Ausblick auf R5](ROADMAP-R5.md).
