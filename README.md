# CP421_ASSIGNMENT_2
## 🔄 Backup Schemes

As part of Assignment 2, the following backup schemes have been researched and analyzed:

### 1. Full Backup
A complete copy of all files and data is taken every time the backup is performed.

- **Execution:** Copies the entire API project and database every time the script runs.
- **Advantages:**
  - Easy to manage and restore.
  - All data is in a single backup file.
- **Disadvantages:**
  - Time-consuming.
  - Requires large storage space.

### 2. Incremental Backup
Only files that have changed since the last backup (whether full or incremental) are copied.

- **Execution:** After an initial full backup, subsequent backups copy only changed files.
- **Advantages:**
  - Very fast and efficient in terms of storage.
- **Disadvantages:**
  - Slower to restore because all incremental backups must be applied in order.

### 3. Differential Backup
Copies files that have changed since the last full backup.

- **Execution:** Every backup includes all changes since the last full backup, regardless of previous differentials.
- **Advantages:**
  - Faster to restore than incremental backup.
- **Disadvantages:**
  - Larger backup size compared to incremental.
  - Slower to perform than incremental as the differential grows daily.
