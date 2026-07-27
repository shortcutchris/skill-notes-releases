# Skill Notes 0.10.0

## English

### iPhone handoff now has a true instant-delivery path

- A compatible iPhone or iPad build sends an additional content-free wake
  signal after its ordinary CloudKit request has been stored.
- Running Macs receive that signal through a lightweight WebSocket connection.
  Direct Apple Push Notification service delivery can also wake a background
  Mac.
- The signal causes one immediate CloudKit fetch. A short bounded retry handles
  the case where the wake arrives just before the encrypted CloudKit record.
- Version 1 broadcasts to every Mac where iPhone handoff is enabled.
- iCloud Settings now shows the instant-delivery and background-wake status of
  this Mac.

CloudKit remains the source of truth. The relay never receives a note ID,
title, body, tag, workspace, task, attachment name, or model setting. It sees
only random event/device identifiers and short-lived timestamps. If the relay
is unavailable, the existing CloudKit push, foreground, wake, and manual sync
paths continue to work.

The currently installed mobile app remains compatible through CloudKit. The
direct fast path becomes active after the matching mobile update is installed.

---

# Skill Notes 0.10.0

## Deutsch

### Die iPhone-Übergabe erhält einen echten Sofortweg

- Ein kompatibler iPhone- oder iPad-Build sendet nach dem Speichern des
  normalen CloudKit-Auftrags zusätzlich ein inhaltsfreies Wecksignal.
- Laufende Macs erhalten dieses Signal über eine leichte
  WebSocket-Verbindung. Eine direkte Apple-Push-Benachrichtigung kann außerdem
  einen Mac im Hintergrund wecken.
- Das Signal startet einen sofortigen CloudKit-Abruf. Eine kurze begrenzte
  Wiederholung deckt den Fall ab, dass das Wecksignal knapp vor dem
  verschlüsselten CloudKit-Datensatz eintrifft.
- Version 1 verteilt an jeden Mac, auf dem die iPhone-Übergabe aktiviert ist.
- Die iCloud-Einstellungen zeigen jetzt Sofortzustellung und
  Hintergrundregistrierung dieses Macs.

CloudKit bleibt die maßgebliche Datenquelle. Die direkte Übergabe erhält
niemals Notiz-ID, Titel, Text, Schlagwort, Arbeitsfläche, Aufgabe,
Anhangsdateiname oder Modelleinstellung. Sie sieht nur zufällige
Ereignis-/Gerätekennungen und kurzlebige Zeitstempel. Falls der Dienst nicht
erreichbar ist, funktionieren CloudKit-Push, Aktivierung, Aufwachen und
manuelle Synchronisierung weiterhin.

Die aktuell installierte mobile App bleibt über CloudKit kompatibel. Der
direkte Schnellweg wird aktiv, nachdem das passende mobile Update installiert
ist.
