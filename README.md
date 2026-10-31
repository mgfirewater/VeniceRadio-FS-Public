# VeniceRadio FS

**Unabhängige Android-Fernbedienung für Radios mit Frontier-Silicon-/Frontier-Smart-Technologies-FSAPI.** Ziel ist, weiterhin funktionsfähige Internetradios – auch ältere Geräte mit Venice 6.5 – unabhängig von der Pflege der bisherigen UNDOK-App bedienen zu können.

Die Software spricht die **FSAPI-Schnittstelle des Radios** an. Sie ist keine UNDOK-Kopie, verwendet keine proprietären UNDOK-Komponenten und ist nicht an einen Radiohersteller gebunden. Welche Funktionen verfügbar sind, bestimmt die tatsächliche FSAPI-Unterstützung des jeweiligen Radios.

## Aktueller Entwicklungsstand – 31. Oktober 2026

| Version | Stand |
| --- | --- |
| **0.4.5-R3** | Referenzstand für den Vergleich und bestehende Gerätetests |
| **0.4.5-R4** | Quellcode-Kandidat fertiggestellt; **37/37 Java-Workflow-Prüfschritte** laut Entwicklungsprotokoll grün. Die R4-Änderungen werden noch auf echten Radios und Smartphones überprüft |
| **0.4.6** | Geplant: responsives Smartphone-Hochformat und schrittweise Mehrsprachigkeit |
| **R5** | Geplant: weitere DLNA-Wiedergabesteuerung (Pause, Fortsetzen, nächster/vorheriger Titel) |

**Wichtig:** Die dokumentierten Java-Tests bestätigen den Quellcode, nicht die vollständige Kompatibilität mit allen FSAPI-Radios. Die Entwicklung und Geräteprüfung erfolgen derzeit in kleinem Rahmen.

## Was VeniceRadio FS bereits im R4-Quellstand enthält

- Fünf Hauptbereiche: **Live, Entdecken, Favoriten, Quelle, Einstellungen**.
- Wiedergabeinformationen, Senderlogos soweit verfügbar, Lautstärke und Standby-Steuerung über FSAPI.
- Navigation und Suche in den vom Radio gelieferten Senderverzeichnissen.
- Favoriten einschließlich Kategorien, Quellenpfaden und getrennt behandelter Radiospeicher; geräteabhängige Verfügbarkeit.
- **„Zuletzt gehört“ pro Radio**, mit bis zu sechs Einträgen; unterschiedliche Empfangsmodi und unterscheidbare Senderwege werden getrennt.
- Sicherere Auflösung ähnlich benannter Sender; keine willkürliche Auswahl des ersten passenden Namens.
- Quellen-/Modusbehandlung für Internetradio, DAB(+) und UKW, **sofern das jeweilige Radio diese Modi meldet**.
- Read-only-Diagnose für unterstützte FSAPI-/WLAN-Informationen; Ergebnisgrenzen und Hinweise bei unvollständigen Abfragen.
- DLNA-Bibliothek und Medienauswahl im bestehenden Entwicklungsstand. Die zusätzlichen Tasten zur DLNA-Wiedergabesteuerung sind **erst für R5** vorgesehen.

Die Oberfläche wurde für R4 vereinheitlicht: zentrale Kachelradien von **12 dp**, einheitliche Kachelabstände, gemeinsame Grundlinien, zweizeilige Beschriftungen und konsistente Ladeanzeige. Schaltflächen und Suchfeld besitzen weiterhin eigene kleinere Radien.

## Orientierung

- [FAQ – häufige Fragen](FAQ.md)
- [Interesse am Projekt und an künftigen Gerätetests](MITMACHEN.md)
- [Änderungen von R3 zu R4](AENDERUNGEN-0.4.5-R3-ZU-R4.md)
- [R4-Status und verbleibende Prüfpunkte](ROADMAP-0.4.5-R4.md)
- [Planung 0.4.6](ROADMAP-0.4.6.md)
- [Planung R5 / DLNA-Steuerung](ROADMAP-R5.md)

## Grenzen und Sicherheit

VeniceRadio FS nutzt die lokale HTTP-basierte FSAPI älterer Radios und sollte nur in einem vertrauenswürdigen Netzwerk verwendet werden. Es gibt keine direkte Anbindung an eine airable-Cloud-API und keinen eigenen Musik-Streaming-Dienst. Nicht jedes Radio unterstützt DAB, UKW, Bluetooth oder dieselben Diagnoseknoten. Es werden keine herstellerspezifischen Hardware-Workarounds eingebaut; die App orientiert sich am gemeldeten Protokollumfang.

**Unabhängiges Projekt:** Keine Zugehörigkeit zu Frontier Smart Technologies, UNDOK, airable, Teufel oder anderen Herstellern.
