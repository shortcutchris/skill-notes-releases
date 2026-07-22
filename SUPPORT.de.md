# Skill Notes Support

Skill Notes Mobile ist eine offline-fähige Notiz- und Aufgaben-App für iPhone und iPad. Ein Skill-Notes-Konto ist nicht erforderlich.

## Vor einer Supportanfrage

1. Prüfe, ob iOS oder iPadOS aktuell ist.
2. Prüfe in Skill Notes den Synchronisierungsstatus, bevor du iCloud-Einstellungen änderst.
3. Aktiviere für das Diktat in den Systemeinstellungen sowohl **Mikrofon** als auch **Spracherkennung** für Skill Notes.
4. Ist die Spracherkennung auf dem Gerät für die gewählte Sprache nicht verfügbar, gib die Notiz oder Aufgabe per Tastatur ein. Skill Notes wechselt nicht stillschweigend zu einer Cloud-Transkription.
5. Sichere wichtige exportierte Markdown-Dateien oder geteilte Dateien vor destruktiver Fehlerbehebung.

## iCloud-Synchronisierung

Die iCloud-Synchronisierung ist optional und verwendet die private CloudKit-Datenbank des Apple Accounts. Prüfe, ob das Gerät mit dem richtigen Apple Account angemeldet und iCloud Drive verfügbar ist. Das Deaktivieren der Synchronisierung löscht lokale oder in der Cloud gespeicherte Daten nicht automatisch.

## Diktatverhalten

- **Notiz diktieren** fügt das Rohtranskript an der Einfügeposition ein und erzeugt niemals automatisch Aufgaben.
- **Aufgaben diktieren** öffnet vor dem Anlegen immer eine bearbeitbare Vorschau.
- Ohne konfiguriertes Strukturierungsmodell bleibt das vollständige Transkript genau eine bearbeitbare Aufgabe.

## Support anfordern

Nutze den öffentlichen [Skill-Notes-Issue-Tracker](https://github.com/shortcutchris/skill-notes-releases/issues/new) und nenne:

- Skill-Notes-Version und Buildnummer;
- iPhone- oder iPad-Modell;
- iOS- oder iPadOS-Version;
- die genauen Schritte zum Reproduzieren; und
- das tatsächliche und das erwartete Verhalten.

Veröffentliche dort keine Notizinhalte, Anhänge, Zugangsdaten, Apple-Account-Daten, Diagnosegeheimnisse oder andere vertrauliche Informationen.

Weitere Informationen enthält die [Datenschutzerklärung für Skill Notes Mobile](PRIVACY.de.md).
