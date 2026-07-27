# Skill Notes 0.9.7

## English

### iPhone handoff reaches the Mac automatically

- Existing Macs migrate once from the older shared CloudKit engine
  subscription state to a dedicated macOS private-database subscription.
- Silent CloudKit pushes can now trigger the running Mac app's fetch path for
  iPhone favorites and **Show on Mac** without requiring **Sync Now**.
- The migration keeps the local notes vault, CloudKit manifest, pending
  changes, conflict mappings, account binding, and last successful sync.
- Later launches reuse the migrated state. No timer or background polling loop
  is introduced.

CloudKit notifications remain a best-effort Apple service and may be
coalesced, but the missing macOS routing subscription no longer prevents their
delivery. Foreground, wake, and manual synchronization remain recovery paths.

---

# Skill Notes 0.9.7

## Deutsch

### iPhone-Übergaben erreichen den Mac automatisch

- Bestehende Macs wechseln einmalig vom älteren gemeinsamen CloudKit-Engine-
  Zustand zu einem eigenen privaten macOS-Datenbank-Abo.
- Stille CloudKit-Pushs können nun den Ladeweg der laufenden Mac-App für
  iPhone-Favoriten und **Auf dem Mac anzeigen** auslösen, ohne dass **Jetzt
  synchronisieren** erforderlich ist.
- Die Migration bewahrt den lokalen Notizspeicher, das CloudKit-Manifest,
  offene Änderungen, Konfliktzuordnungen, Kontobindung und den letzten
  erfolgreichen Sync.
- Spätere Starts verwenden den migrierten Zustand weiter. Es wird weder ein
  Timer noch eine Hintergrund-Abfrageschleife ergänzt.

CloudKit-Benachrichtigungen bleiben ein bestmöglicher Apple-Dienst und können
zusammengefasst werden. Das fehlende macOS-Routing-Abo verhindert ihre
Zustellung jedoch nicht länger. Aktivierung, Aufwachen und die manuelle
Synchronisierung bleiben Wiederherstellungswege.
