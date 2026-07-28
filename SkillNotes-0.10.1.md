# Skill Notes 0.10.1

## English

### Faster iPhone handoff after a fresh install

- Skill Notes now waits until the encrypted iCloud vault has confirmed the
  shared instant-delivery channel before connecting to it.
- A fresh Mac and iPhone can no longer temporarily use different locally
  generated channels during their first synchronization.
- Account changes, sign-out, and iCloud zone recovery safely invalidate the
  old confirmation and reconnect only after the new cloud context is ready.
- The Mac confirms its WebSocket connection with a real server response and
  keeps a bounded fallback window when the wake signal arrives just before
  the CloudKit record.
- Rapid relay reconfiguration no longer risks removing the current Mac's
  background notification registration.

CloudKit remains the source of truth and the relay remains content-free. The
verification path uses synthetic notes and reports only states, checks, and
latency—never relay credentials, note identifiers, or authored content.

The matching mobile sender improvement has been verified in the iOS Simulator
but is not part of this macOS update.

---

# Skill Notes 0.10.1

## Deutsch

### Schnellere iPhone-Übergabe nach einer Neuinstallation

- Skill Notes verbindet sich erst dann mit dem Sofortkanal, wenn der
  verschlüsselte iCloud-Tresor die gemeinsame Identität bestätigt hat.
- Ein frisch installierter Mac und ein iPhone können während der ersten
  Synchronisierung nicht mehr vorübergehend unterschiedliche lokal erzeugte
  Kanäle verwenden.
- Accountwechsel, Abmeldung und die Wiederherstellung der iCloud-Zone
  verwerfen die alte Bestätigung sicher und verbinden erst wieder, wenn der
  neue Cloud-Kontext bereit ist.
- Der Mac bestätigt die WebSocket-Verbindung mit einer echten Serverantwort
  und verwendet weiterhin ein begrenztes Fallback-Fenster, falls das
  Wecksignal knapp vor dem CloudKit-Datensatz eintrifft.
- Eine schnelle Relay-Neukonfiguration kann die
  Hintergrundregistrierung des aktuellen Macs nicht mehr versehentlich
  entfernen.

CloudKit bleibt die maßgebliche Datenquelle und das Relay bleibt inhaltsfrei.
Der Prüfpfad verwendet synthetische Notizen und protokolliert nur Zustände,
Prüfergebnisse und Latenzen – niemals Relay-Zugangsdaten, Notizkennungen oder
verfasste Inhalte.

Die passende Verbesserung des mobilen Senders wurde im iOS-Simulator geprüft,
ist aber nicht Bestandteil dieses macOS-Updates.
