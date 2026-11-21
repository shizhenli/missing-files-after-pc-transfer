---
title: "External Drive Files Missing After Transfer: Fixing a Partial Copy on Windows"
description: "External drive files missing after transfer? Learn how to check copy logs, verify hidden files, and restore user folders on your new Windows PC."
seo_title: "External Drive Files Missing After Transfer: Fix a Partial Copy"
seo_description: "External drive files missing after transfer? Learn how to check copy logs, verify hidden files, and restore user folders on your new Windows PC."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-21T14:37:04+08:00
publishDate: 2026-11-21T14:37:04+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to an external drive, but after transferring them to the new PC, some folders or files are simply not there.

## Check the Copy Log and Source Folder

First, reconnect the external drive to the old PC. Open File Explorer, right-click the drive, and choose Properties. Compare the used space with the total size of the folders you copied. If the drive shows significantly less data than expected, the first copy stopped early. Next, open the source user folder (C:\Users\YourName) and confirm that Desktop, Documents, and Downloads actually contain files. If they appear empty, enable hidden items via View > Show > Hidden items. A folder that looks empty but has size is often a permissions or junction issue, not a missing file.

## Verify Hidden and System Files on the New PC

On the new PC, open the destination folder and enable hidden items again. Check whether the missing folders exist but are marked hidden. Also look for folders named "Desktop" inside OneDrive or under a different user profile. If you see a folder with the right name but zero bytes, the copy created the folder structure without the contents.

## Run a Verification Test

Create a small test folder on the external drive with three files. Copy it to the new PC using File Explorer, then open each file. If the test files appear, the drive and connection are fine, and the original transfer was incomplete. If they do not appear, the destination path or permissions are blocking the copy.

## Rollback and Recovery

Do not delete the external drive copy. Re-copy the missing user folders from the old PC using a direct USB connection, and choose "Replace the files in the destination" only after confirming the source is complete. If the old PC is unavailable, use Windows File History or a backup image to restore the folders. For a controlled diagnosis of your **external drive files missing after transfer**,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
