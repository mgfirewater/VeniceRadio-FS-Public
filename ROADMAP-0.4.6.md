# VeniceRadio FS – Planung 0.4.6

> **Noch nicht für 0.4.6 implementiert oder freigegeben.** R4 ist der Stabilitäts- und Konsistenzabschluss. Der Umfang kann sich nach dem Gerätetest ändern.

## Responsive Smartphone-Benutzeroberfläche

- [ ] Entdecken-Kachelraster und Seitenmenge aus tatsächlich verfügbarer Displayhöhe bestimmen, statt einen festen Wert auf alle Smartphones anzuwenden
- [ ] Auf dem Referenz-Smartphone im Hochformat nach Möglichkeit neun vollständige Zweispaltenzeilen zeigen; auf anderen Geräten eine passende Zahl ohne abgeschnittene Zeilen
- [ ] Suchfeld, Breadcrumb und Seitennavigation stabil halten; keine verschobenen Grundlinien, keine abweichenden Radien oder ungleichen Abstände
- [ ] Letzte Suche, Verzeichnisweg und Seite beim Ansichtswechsel erhalten; keine unnötigen FSAPI-Abfragen
- [ ] Unterschiedliche Systemschriftgrößen und Bildschirmauflösungen testen

## Mehrsprachigkeit

- [ ] Texte in übersetzbare Android-Ressourcen übernehmen
- [ ] Systemsprache verwenden, sofern eine Übersetzung vorliegt; optionale manuelle Sprachwahl
- [ ] Fallback-Sprache bei fehlender Übersetzung vorsehen
- [ ] Radioseitig gelieferte Sendernamen und Metadaten unverändert lassen
- [ ] Übersetzte längere Beschriftungen im adaptiven Layout prüfen

## Spätere optionale Darstellungen

- [ ] Tablet-Layout
- [ ] Querformat/Wide-Mode

**Abgrenzung:** Neue DLNA-Pause-/Weiter-/Zurück-Steuerung ist für [R5](ROADMAP-R5.md) vorgesehen. Sie gehört nicht automatisch zu 0.4.6. [R4-Status](ROADMAP-0.4.5-R4.md).
