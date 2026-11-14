---
title: "Files Missing After PC Transfer: Why the First Copy Leaves User Folders Empty"
description: "First copy finished but user folders are empty on the new PC? Run these checks to confirm whether files were skipped, hidden, or left on the old drive."
seo_title: "Files Missing After PC Transfer: Diagnose an Empty First Copy"
seo_description: "First copy finished but user folders are empty on the new PC? Run these checks to confirm whether files were skipped, hidden, or left on the old drive."
keywords:
  - "files missing after pc transfer"
date: 2026-11-14T19:18:45+08:00
publishDate: 2026-11-14T19:18:45+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to the new PC, the progress bar finished, but now Documents, Pictures, or Desktop appear empty on the destination.

## Confirm what the first copy actually contained

Open File Explorer on the new PC and navigate to `C:\Users\<your-username>`. Right-click each user folder, choose Properties, and read the Size and Contains values. A folder showing 0 bytes and 0 files means the copy skipped its contents rather than losing them later. Next, check the source PC the same way. If the source folders hold data but the destination folders are empty, the transfer stopped at the folder shell.

## Check for hidden and redirected folders

In File Explorer, enable View > Show > Hidden items. Some migration tools copy only visible items, so a folder full of hidden files can look empty. Also right-click a user folder, open Properties > Location, and confirm the path points to the new PC's drive, not a leftover network or old-drive path.

## Verification test

Create a test file on the old PC inside Documents, then copy that single file manually to the matching folder on the new PC. If it appears, the folder structure is intact and only the bulk copy failed. If it does not appear, the destination folder is redirected or read-only.

## Recovery note

Do not delete anything on the old PC yet. Recopy the missing folders directly from the old drive to the new one, overwriting the empty shells. If the source drive was already wiped or the folders remain absent, stop and

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before further writes, since **files missing after pc transfer** can often still be recovered from the original disk.
