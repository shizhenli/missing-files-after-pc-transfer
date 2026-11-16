---
title: "External Drive Files Missing After Transfer: Fixing the Incomplete Copy"
description: "External drive files missing after transfer? Diagnose an incomplete copy during PC migration, verify with a checksum test, and recover missing files safely."
seo_title: "External Drive Files Missing After Transfer: Fix the Incomplete Copy"
seo_description: "External drive files missing after transfer? Diagnose an incomplete copy during PC migration, verify with a checksum test, and recover missing files safely."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-16T10:00:05+08:00
publishDate: 2026-11-16T10:00:05+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to an external drive, moved them to the new PC, and now the folders look empty or incomplete. This is a common sign that the first copy stopped early or skipped files, not that the files are gone. Here is how to diagnose and fix it.

## Check the source and destination counts

On the old PC, open the external drive in File Explorer. Right-click the user folder, choose Properties, and note the item count and total size. Do the same on the new PC. If the destination count is lower, the copy was incomplete. Also check whether hidden files are visible: in File Explorer, open View and enable Hidden items. If AppData or dot-folders are missing, the copy likely skipped them.

## Look for copy errors and free space

Review the external drive for a copy log or error dialog you may have dismissed. Confirm the drive has enough free space for the full folder size. If the drive is formatted as FAT32, files over 4 GB will be skipped, which can leave folders looking empty. Check the drive's file system in Properties.

## Run a verification test

Create a small test folder on the old PC with three files, copy it to the external drive, then to the new PC. Compare file counts and open each file. If the test passes, the issue is specific to the large user folder; recopy it in smaller subfolders and confirm each one before moving on.

## Rollback and recovery

Do not delete the original files on the old PC until the new copy is verified. If the **external drive files missing after transfer**, recopy from the old PC rather than trying to rebuild from partial data. Keep the old PC unchanged until the new one is confirmed complete.

If the counts still do not match,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before making further changes.
