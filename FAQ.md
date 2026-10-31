# VeniceRadio FS – FAQ

**Stand: 31. Oktober 2026.** Angaben zum implementierten R4-Quellstand sind von bereits auf echten Geräten bestätigten Funktionen zu unterscheiden.

## Wozu dient VeniceRadio FS?

Zur Bedienung kompatibler Internetradios über die lokale FSAPI-Schnittstelle. Das Radio spielt selbst ab; die Android-App ist Fernbedienung und Benutzeroberfläche.

## Welche Radios werden unterstützt?

Entscheidend sind **FSAPI und die vom Radio gemeldeten Fähigkeiten**, nicht die Marke. Besonders relevant sind ältere Venice-6.5-Geräte. Die konkrete Kompatibilität muss je Radio und Firmware getestet werden.

## Was ist mit UNDOK und OKTIV?

VeniceRadio FS entsteht als unabhängige Alternative für kompatible FSAPI-Radios. Ältere Venice-6.5-Geräte gehören nicht zum regulären OKTIV-Unterstützungsumfang. Der Entwicklungsstand von VeniceRadio FS bedeutet nicht, dass alle früheren UNDOK-Funktionen bereits vollständig nachgebildet wurden.

## Ist R4 schon veröffentlicht?

**Nein, nicht als öffentlich bestätigte APK.** Für den R4-Quellcode wurden 37/37 Java-Workflow-Schritte dokumentiert; der signierte Android-Build und die abschließenden Tests auf echten Radios sind eigenständige nächste Schritte. Eine öffentliche APK-Verteilung ist hier nicht eingerichtet.

## Kann ich R4 über R3 installieren?

Die R4-Quellkonfiguration sieht **Version 0.4.5-R4, versionCode 57** und die unveränderte Android-Anwendungskennung vor. Ein Update ohne Datenverlust setzt zusätzlich voraus, dass die neue APK tatsächlich mit **demselben Signaturschlüssel** wie die bestehende Installation signiert ist. Die konkrete APK muss noch überprüft werden.

## Werden meine Favoriten und Senderverläufe beim Update gelöscht?

Die R4-Migration ist darauf ausgelegt, vorhandene Favoriten und Ordner zu erhalten. „Zuletzt gehört“ ist nun je Radio getrennt. Alte Verlaufseinträge, die sich keinem Radio sicher zuordnen lassen, bleiben gespeichert, werden aber nicht mehr angezeigt. Ein vollständiger Update-Test auf Geräten ist noch ausstehend.

## Warum können zwei Kacheln gleich heißen?

Internetradio, DAB und UKW sowie verschiedene Verzeichniswege können unterschiedliche Senderidentitäten mit gleichem sichtbarem Namen ergeben. R4 trennt sie intern. Eine zusätzliche sichtbare Kennzeichnung gleicher Namen aus unterschiedlichen Modi ist noch nicht gestaltet; die Kachel bleibt zweizeilig.

## Unterstützt die App DAB+, UKW und Bluetooth?

Nur, wenn das angeschlossene Radio diese Empfangsarten beziehungsweise Eingänge per FSAPI anbietet. VeniceRadio FS empfängt oder dekodiert die Rundfunksignale nicht selbst und übernimmt auch keine Bluetooth-Audiokopplung.

## Gibt es DLNA-Unterstützung?

DLNA-Bibliotheksnavigation, Medienauswahl und Wiedergabegrundlagen sind im Entwicklungsstand vorhanden. Die zusätzliche Bedienung über **Pause, Fortsetzen, nächster und vorheriger Titel** ist für **R5** vorgesehen und darf nicht als fertig getestete R4-Funktion verstanden werden.

## Gibt es eine eigene airable-Anmeldung oder Streaming-Konten?

Nein. Die App verwendet die vom Radio bereitgestellten FSAPI-Verzeichnisse und benötigt keinen eigenen airable-Account.

## Was muss ich für einen Test bereitstellen?

Radio mit FSAPI, Android-Telefon und gemeinsames lokales Netzwerk. Besonders hilfreich sind beobachtete Abweichungen bei DAB/UKW-Modi, WLAN-Diagnose, identischen Sendernamen und Presets. Details: [Mitmachen](MITMACHEN.md).

## Wo melde ich Fehler?

Über die vom Projekt bekanntgegebenen Testkanäle beziehungsweise die öffentliche Projektkommunikation. Bitte niemals Radio-PINs, Zugangsdaten, Session-IDs oder ungekürzte private Netzwerkdaten veröffentlichen.
