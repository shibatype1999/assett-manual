# Backing Up and Restoring Data
<!-- position: 9 -->
<!-- description: Local backups, auto backups, exporting to a file, and how to restore your data. -->

All of your data is stored on your device.
We recommend backing up regularly in case you change devices or something goes wrong.

Backups are under **Settings** → **Backup**.

![Backup screen](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/backup.png)

| Method | Saved to | Best for |
| --- | --- | --- |
| Local Backup | Inside the app | A temporary copy before making big changes |
| Auto Backup (Premium) | Inside the app | Regular backups |
| Export Data (Premium) | A file (iCloud Drive, etc.) | Changing devices, long-term storage |

## Local Backup

Saves a copy of your current data inside the app. No file sharing is involved.

### Saving

1. Tap **Local Backup**.
2. When "Backup created" appears, you're done. The **Last Backup** date and time are shown below the button.

Each time you save, a new local backup is added.

### Restoring from the latest backup

1. Tap **Restore from Local**.
2. The confirmation dialog shows the date and time of the latest backup. Tap **Restore**.

### Restoring from the backup list (Premium feature)

1. Tap **Restore from backup list**.
2. Saved backups are listed with their date and time, whether they are **Auto** or **Manual**, and the number of assets and records.
3. Tap the backup you want to restore, then tap **Restore** in the confirmation dialog.

You can delete backups you no longer need with the trash icon in the list.

![Backup list](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/backup-list.png)

> **Caution**
> - Restoring overwrites your current data.
> - Local backups (including auto backups) are stored inside the app, so **they are deleted if you delete the app**. To change devices, use **Export Data**.

## Auto Backup (Premium feature)

Creates local backups automatically at a set interval.

1. Tap **Auto Backup**.
2. Turn on **Enable auto backup**. The first backup is created when you turn it on.
3. Choose an **Interval**: **Daily**, **Weekly**, or **Monthly**.
4. Under **Delete old auto backups**, choose when old auto backups are deleted.

![Auto Backup](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/auto-backup.png)

### When backups are created

Auto backups do not run at a fixed time. **When you open (or return to) the app**, a backup is created if the chosen interval has passed since the last auto backup.

| Interval | When a backup is created |
| --- | --- |
| Daily | The first time you open the app 24 hours or more after the last auto backup (e.g. last at 14:30 → on the first launch after 14:30 the next day) |
| Weekly | The first time you open the app 7 days or more after the last auto backup |
| Monthly | The first time you open the app after the same day and time in the following month. If that day doesn't exist, the last day of the month is used (e.g. 1/31 → 2/28) |

The screen shows the time of the last auto backup and the next scheduled one.

### Deleting old auto backups

Choose one of the following:

- Keep all
- Delete older than N days (30, 90, or 180 days)
- Keep latest N (10, 20, or 30)
- Delete oldest when over N MB total (10, 50, or 100 MB)

**Only auto backups** are deleted automatically; backups you created manually are kept.
With **Keep all**, storage use keeps growing, so delete unneeded backups from the list as needed. The screen shows the total size and number of auto backups.

## Export Data (Premium feature)

Exports your data as a single file (`asset-YYYYMMDD-HHMMSS.json`) that you can save to iCloud Drive and other services.
You can also set a password to export the file encrypted.

### On iOS

1. Tap **Export Data**.
2. Choose how to export.
   - **Export encrypted** – Only people who know the password can restore it (recommended).
   - **Export without encryption** – Anyone can read the file contents.
3. If you chose **Export encrypted**, enter the same password (at least 4 characters) in **Password** and **Enter again**, then tap **Encrypt and export**.
4. The share sheet opens.
5. Choose where to save.
   - **To save to iCloud Drive** – Tap **Save to Files**, choose a folder in **iCloud Drive**, then tap **Save**.
   - **To save to another app** – Choose an app such as Google Drive and follow the on-screen instructions.

![Share sheet](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/backup-share-sheet.png)

> **Caution**
> - The password is not saved in the app and is not sent to the operator. **If you forget the password, the encrypted file cannot be restored.**
> - A file exported without encryption contains your asset names and balances as they are. Be careful where you save or share it.

## Import Data (Premium feature)

Restores your data from an exported file.

### On iOS

1. Tap **Import Data**.
2. The file picker opens. Choose the exported file (`asset-….json`).
3. If the file is encrypted, "This file is encrypted" appears. Enter the password you set when exporting.
4. Tap **Restore** in the confirmation dialog.
5. When "Restored successfully" appears, you're done.

> **Caution**
> - Importing overwrites your current data.
> - Only files exported from this app can be imported. If a file can't be read, "Restore failed" is shown.
> - If the password is wrong, "Wrong password" is shown.

## What is included in a backup

| Included | Not included |
| --- | --- |
| Assets | Default currency |
| Records (balances, dates and times, subcategories, memos) | Display format and date format |
| Categories | Theme and theme color |
| Subcategories | Dashboard panel layout |
| Asset goal | Auto backup settings |
| Display language | |
| Custom currencies | |
| Currency rate settings | |

After restoring, set up the settings that are not included again as needed.
