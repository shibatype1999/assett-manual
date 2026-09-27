# Backing Up and Restoring Data
<!-- position: 7 -->
<!-- description: How to back up (locally or to a file) and restore your data. -->

All of your data is stored on your device.
We recommend backing up regularly in case you change devices or something goes wrong.

Backups are under **Settings** → **Backup**.

![Backup screen](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/backup.png)

There are two ways to back up.

| Method | Saved to | Best for |
| --- | --- | --- |
| Local Backup | Inside the app | A temporary copy before making big changes |
| Export Data | A file (iCloud Drive, etc.) | Changing devices, long-term storage |

## Local Backup

Saves a copy of your current data inside the app. No file sharing is involved.

### Saving

1. Tap **Local Backup**.
2. When "Backup created" appears, you're done. The **Last Backup** date and time are shown below the button.

Only one local backup is kept. Saving again overwrites the previous one.

### Restoring

1. Tap **Restore from Local**.
2. Tap **Restore** in the confirmation dialog.

> **Caution**
> - Restoring overwrites your current data.
> - Local backups are stored inside the app, so **they are deleted if you delete the app**. To change devices, use **Export Data** below.

## Export Data (save to a file)

Exports your data as a single file (`asset-YYYYMMDD-HHMMSS.json`) that you can save to iCloud Drive and other services.

### On iOS

1. Tap **Export Data**.
2. The share sheet opens.
3. Choose where to save.
   - **To save to iCloud Drive** – Tap **Save to Files**, choose a folder in **iCloud Drive**, then tap **Save**.
   - **To save to another app** – Choose an app such as Google Drive and follow the on-screen instructions.

![Share sheet](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/backup-share-sheet.png)

## Import Data (restore from a file)

Restores your data from an exported file.

### On iOS

1. Tap **Import Data**.
2. The file picker opens. Choose the exported file (`asset-….json`).
3. Tap **Restore** in the confirmation dialog.
4. When "Restored successfully" appears, you're done.

> **Caution**
> - Importing overwrites your current data.
> - Only files exported from this app can be imported. If a file can't be read, "Restore failed" is shown.

## What is included in a backup

| Included | Not included |
| --- | --- |
| Categories | Subcategory list (added or renamed subcategories) |
| Records (balances, dates, memos, etc.) | Default currency |
| Asset goal | Display format (decimal places, rounding) |
| Display language | Theme and theme color |
| Custom currencies | |
| Currency rate settings | |

After restoring, set up the settings that are not included again as needed.
