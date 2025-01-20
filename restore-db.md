# How to restore DB

1. Change the BACKUP_FILE env inside the [postgres-restore](./db/restore-backup.yaml) to the name of the backup file you want to apply to the db. For example:

```bash
- name: BACKUP_FILE
  value: "2025-01-20/backup.sql"
```

2. Run the job from the ArgoCD UI
