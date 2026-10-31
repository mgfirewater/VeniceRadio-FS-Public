# VeniceRadio FS 0.4.5 R4 – geplante Nacharbeiten

> **To-do / noch nicht umgesetzt.** Die erste Geräteprüfung von 0.4.5 R3 hat Vorrang.

## WLAN-Diagnose

- [ ] Prüfen, welche **lesbaren** FSAPI-WLAN-Diagnosewerte verschiedene Radiomodelle und Firmwarestände tatsächlich liefern.
- [ ] BSSID, Signalstärke und mögliche Repeater-Zuordnung nur dann anzeigen, wenn verlässliche Gerätedaten vorliegen.
- [ ] Nicht unterstützte Diagnoseknoten ohne Änderung der Hauptsitzung behandeln.
- [ ] Prüfen, ob die länger dauernde WLAN-Diagnose den vorhandenen dezenten Ladeindikator anzeigen soll.

**Abgrenzung:** Die in 0.4.5 R3 korrigierte Deprecation-Warnung betraf ausschließlich den Java-Aufruf `URL(String)`. Sie war **keine** veraltete WLAN- oder Android-API und ist kein offener R4-Fehler.

## DAB / DAB+

- [ ] Eigenständiges DAB(+)-Symbol gestalten, ohne den freigegebenen Internetradio-Funkturm zu ändern.
- [ ] Quellenumschaltung und Sendernavigation auf geeigneten DAB-/DAB+-fähigen Radios testen.
- [ ] Geräteabhängige Unterstützung klar kennzeichnen; das Haupttestgerät besitzt keinen DAB-Empfänger.

Mehrsprachigkeit und die responsive Darstellung für klassische Smartphones im Hochformat sind separat für **0.4.6** geplant: [Roadmap 0.4.6](ROADMAP-0.4.6.md).
