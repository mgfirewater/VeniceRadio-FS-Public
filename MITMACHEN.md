# Interesse am Projekt und an künftigen Gerätetests

**Stand 31. Oktober 2026.** VeniceRadio FS wird derzeit in einem kleinen privaten Rahmen entwickelt und getestet. Es gibt noch keine größere organisierte Testgruppe. Wer ein kompatibles FSAPI-Internetradio besitzt und sich für einen späteren Test interessiert, kann über die öffentliche Projektkommunikation Kontakt aufnehmen, sofern dort ein Kontaktweg angeboten wird.

Ziel ist, die Unterstützung **über tatsächlich gemeldete FSAPI-Fähigkeiten statt über Hersteller-Sonderwege** abzusichern.

## Bereiche, zu denen Rückmeldungen später besonders hilfreich wären

1. **Geräteverbindung:** Modell, Firmwarestand, vom Radio angebotene FSAPI-Quellen und Stabilität beim Wiederverbinden.
2. **Entdecken und Favoriten:** verschachtelte Verzeichnisse, Suchergebnisse, Senderlogos, Zurück-Navigation und Favoritenordner.
3. **„Zuletzt gehört“:** Wechsel zwischen zwei Radios; identische Namen bei Internet/DAB/UKW; regionale Varianten und Einträge mit Zusätzen wie „laut.fm“.
4. **WLAN-Diagnose:** nur lesende Informationen, Scanlisten auch über 25 Einträge, Hinweise bei fehlenden oder unvollständigen Werten.
5. **Oberfläche:** Kachelgrundlinien, zweizeilige Namen, Seitenbedienung und Performance auf unterschiedlichen Smartphone-Größen.
6. **Radiospeicher:** vorerst **nur auslesen und vorhandene belegte Plätze vergleichen**. Kein unbeaufsichtigtes Überschreiben und keine Suchläufe.

## Grundsätze für spätere Tests

- Testschritte werden erst nach Absprache durchgeführt; insbesondere **keine** Werksresets, DAB-Suchläufe, WLAN-Änderungen oder Schreibtests an Radiospeichern ohne ausdrückliche Freigabe.
- Bei Rückmeldungen helfen: Gerätemodell, Firmware, Android-Version, genaue Bedienfolge, erwartetes und tatsächliches Ergebnis.
- In Diagnoseauszügen **PIN, Session-ID, private IP, WLAN-Namen und BSSID** vor einer Veröffentlichung entfernen oder ausreichend unkenntlich machen.
- Öffentlich verwendete App-Screenshots werden erst nach Kontrolle der Piktogramme, Favoriten-/Ordnernavigation und DLNA-Coverdarstellung ausgewählt.

## Was bereits feststeht

Die Entwicklung nutzt eine gemeinsame FSAPI-Implementierung. Unterschiedliche Geräte können unterschiedliche Knoten und Menüs anbieten; daraus wird kein Hersteller-Sonderfall abgeleitet. Rückmeldungen sollen helfen, das reale Protokollverhalten zu dokumentieren.

Siehe auch [FAQ](FAQ.md), [R4-Status](ROADMAP-0.4.5-R4.md) und [Ausblick auf R5](ROADMAP-R5.md).
