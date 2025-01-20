# Manually trigger the db-backup

1. Run the following command

```bash
 sudo kubectl create job --from=cronjob/postgres-backup manual-backup-job
```
