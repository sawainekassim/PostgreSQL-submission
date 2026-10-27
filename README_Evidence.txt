EVIDENCE SCREENSHOT CHECKLIST

Save screenshots in this folder using the suggested filenames. Capture the PowerShell command and its output in the same image where possible. Do not include your PostgreSQL password or any other secret in a screenshot.

01_logical_restore.png
  Show the bootcamp_check student count query returning 5 rows.

02_physical_backup_verification.png
  Show pg_verifybackup reporting: backup successfully verified.

03_wal_archiver_status.png
  Show pg_stat_archiver with the last archived WAL and failed_count = 0.

04_pitr_recovery_rows.png
  Show the port 5433 query with in_recovery = t and restored_rows = 2, or the SELECT listing IDs 1 and 2.

05_pitr_deleted_primary.png (if required)
  Show the primary-side pitr_demo count result of 0 after the simulated deletion. Do not re-run DELETE just for this screenshot.

06_standby_receiver_streaming.png
  Show pg_stat_wal_receiver on port 5434 with status = streaming and sender_port = 5432.

07_primary_replication_status.png
  Show pg_stat_replication on port 5432 with state = streaming and sync_state = async.

08_replication_test_row.png
  Show the SELECT result on port 5434 returning ID 3, Replication test record.

If the lecturer's instructions require different evidence, follow the original instructions. Take screenshots of outputs you already have, if available in scrollback/history; do not claim a screenshot exists until you have saved it.
