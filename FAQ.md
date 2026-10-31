# VeniceRadio FS – FAQ

**Stand: 31. Oktober 2026.** Angaben zum implementierten R4-Quellstand sind von bereits auf echten Geräten bestätigten Funktionen zu unterscheiden.

## Wozu dient VeniceRadio FS?

Zur Bedienung kompatibler Internetradios über die lokale FSAPI-Schnittstelle. Das Radio spielt selbst ab; die Android-App ist Fernbedienung und Benutzeroberfläche.

## Welche Radios werden unterstützt?

Entscheidend sind **FSAPI und die vom Radio gemeldeten Fähigkeiten**, nicht die Marke. Besonders relevant sind ältere Venice-6.5-Geräte. Die konkrete Kompatibilität muss je Radio und Firmware getestet werden.

## Was ist mit UNDOK und OKTIV?

VeniceRadio FS entsteht als unabhängige Alternative für kompatible FSAPI-Radios. Ältere Venice-6.5-Geräte gehören nicht zum regulären OKTIV-Unterstützungsumfang. Der Entwicklungsstand von VeniceRadio FS bedeutet nicht, dass alle früheren UNDOK-Funktionen bereits vollständig nachgebildet wurden.

## Wie weit ist die Entwicklung von R4?

Die Korrekturen sind im aktuellen R4-Quellstand integriert. Laut Entwicklungsprotokoll bestanden 37/37 Java-Workflow-Prüfschritte. Die praktische Überprüfung mit unterschiedlichen FSAPI-Radios und Smartphones ist noch nicht abgeschlossen.

## Wie werden vorhandene Favoriten und Senderverläufe behandelt?

Die R4-Migration ist darauf ausgelegt, vorhandene Favoriten und Ordner zu erhalten. „Zuletzt gehört“ ist nun je Radio getrennt. Alte Verlaufseinträge, die sich keinem Radio sicher zuordnen lassen, bleiben gespeichert, werden aber nicht mehr angezeigt. Die Umsetzung dieser Datenübernahme muss in der laufenden Geräteprüfung bestätigt werden.

## Warum können zwei Kacheln gleich heißen?

Internetradio, DAB und UKW sowie verschiedene Verzeichniswege können unterschiedliche Senderidentitäten mit gleichem sichtbarem Namen ergeben. R4 trennt sie intern. Eine zusätzliche sichtbare Kennzeichnung gleicher Namen aus unterschiedlichen Modi ist noch nicht gestaltet; die Kachel bleibt zweizeilig.

## Unterstützt die App DAB+, UKW und Bluetooth?

Nur, wenn das angeschlossene Radio diese Empfangsarten beziehungsweise Eingänge per FSAPI anbietet. VeniceRadio FS empfängt oder dekodiert die Rundfunksignale nicht selbst und übernimmt auch keine Bluetooth-Audiokopplung.

## Gibt es DLNA-Unterstützung?

DLNA-Bibliotheksnavigation, Medienauswahl und Wiedergabegrundlagen sind im Entwicklungsstand vorhanden. Die zusätzliche Bedienung über **Pause, Fortsetzen, nächster und vorheriger Titel** ist für **R5** vorgesehen und darf nicht als fertig getestete R4-Funktion verstanden werden.

## Gibt es eine eigene airable-Anmeldung oder Streaming-Konten?

Nein. Die App verwendet die vom Radio bereitgestellten FSAPI-Verzeichnisse und benötigt keinen eigenen airable-Account.

## Gibt es schon eine größere Testgruppe?

Nein. Die Entwicklung und Prüfung erfolgen derzeit in kleinem privatem Rahmen. Rückmeldungen weiterer interessierter Besitzer FSAPI-kompatibler Radios wären willkommen; es gibt noch keine organisierte externe Testgruppe. Hinweise zu interessanten Geräten und Prüfbereichen stehen unter [Mitmachen](MITMACHEN.md).

## Wo melde ich Fehler?

Über die öffentliche Projektkommunikation, soweit dafür ein Kontaktweg genannt ist. Bitte niemals Radio-PINs, Zugangsdaten, Session-IDs oder ungekürzte private Netzwerkdaten veröffentlichen.
