# Skill Notes 0.8.14

This reliability update completes the repair path for iCloud changes that
previously remained at 0 of N.

When CloudKit reports a missing record or reference target, Skill Notes now
rebuilds the affected record together with its parent note and retries the
upload in a bounded sequence. Only stale CloudKit system metadata is reset;
note content, attachments, revisions, local history, and the durable pending
queue remain untouched.

Repairs stop after two failed attempts, so a damaged remote relationship can
never become another background loop. Privacy-safe diagnostics contain only
the CloudKit error code, record kind, and attempt number.

When a record already exists on another device, Skill Notes now fetches its
complete server version before merging it. This ensures revision and
attachment assets are downloaded and verified before the pending local entry
is acknowledged.

## Deutsch

Dieses Zuverlässigkeitsupdate vervollständigt den Reparaturpfad für
iCloud-Änderungen, die zuvor bei 0 von N stehen blieben.

Wenn CloudKit einen fehlenden Datensatz oder ein fehlendes Referenzziel
meldet, baut Skill Notes den betroffenen Datensatz jetzt gemeinsam mit seiner
übergeordneten Notiz neu auf und wiederholt den Upload in einer begrenzten
Folge. Dabei werden nur veraltete CloudKit-Systemdaten zurückgesetzt;
Notizinhalte, Anhänge, Revisionen, lokaler Verlauf und die dauerhafte
Warteschlange bleiben unverändert.

Nach zwei fehlgeschlagenen Reparaturversuchen stoppt die Wiederholung, sodass
aus einer beschädigten Remote-Beziehung keine neue Hintergrundschleife
entstehen kann. Die datensparsame Diagnose enthält ausschließlich den
CloudKit-Fehlercode, die Datensatzart und die Versuchsnummer.

Existiert ein Datensatz bereits auf einem anderen Gerät, lädt Skill Notes die
vollständige Server-Version vor dem Zusammenführen neu. Dadurch werden
Revisionen und Anhänge heruntergeladen und geprüft, bevor der lokale Eintrag
aus der Warteschlange bestätigt wird.
