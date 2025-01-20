# How to restore DB

1. Change the BACKUP_FILE env inside the [postgres-restore](./db/restore-backup.yaml) to the name of the backup file you want to apply to the db. For example:

```yaml
- name: BACKUP_FILE
  value: "/backup/2025-01-20/backup.sql"
```

2. Change the suspend inside the [postgres-restore](./db/restore-backup.yaml) to `false`:

```yaml
suspend: false
```

3. Sync ArgoCD to run the job.
