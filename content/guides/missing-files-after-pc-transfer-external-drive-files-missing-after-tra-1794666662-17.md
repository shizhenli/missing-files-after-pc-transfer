---
title: "External Drive Files Missing After Transfer: Verifying the Copy"
description: "Fix external drive files missing after transfer on Windows by verifying the copy, checking hidden folders, and restoring from the source drive safely."
seo_title: "External Drive Files Missing After Transfer: Verify the Copy"
seo_description: "Fix external drive files missing after transfer on Windows by verifying the copy, checking hidden folders, and restoring from the source drive safely."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-26T07:59:17+08:00
publishDate: 2026-11-26T07:59:17+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to an external drive, moved them to the new PC, and now the folders look empty or absent.

## Check the source before touching the destination

Reconnect the external drive to the old PC. Open File Explorer, right-click the drive, and choose Properties. Compare the used space figure with what you expect from your user folders. If the used space is far below the size of your data, the copy stopped early. Next, open the destination folder and enable View > Show > Hidden items. Missing Desktop, Documents, or AppData folders are often present but hidden. If they appear, the transfer worked; the new PC is simply not displaying them.

## Run a verification test

On the old PC, open Command Prompt and run:

`robocopy "C:\Users\YourName" "E:\Backup\YourName" /L /E /XD AppData`

The /L switch lists what would be copied without changing anything. If the list shows files that are absent on the external drive, the first copy was incomplete. This is the most common cause of **external drive files missing after transfer**.

## Recover without overwriting

Do not copy back over the old profile. Instead, copy the missing folders from the old PC to a new folder on the external drive, then move that folder to the new PC. Keep the original source untouched until you confirm every file opens. If the old PC is already wiped, stop using the external drive and ask for help before writing anything else to it.

Once the verification list matches the destination, your transfer is complete. If it does not,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before repeating the copy.
