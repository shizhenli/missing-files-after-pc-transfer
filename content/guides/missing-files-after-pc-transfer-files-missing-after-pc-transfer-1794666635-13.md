---
title: "Files Missing After PC Transfer: Confirming the Copy Covered All User Folders"
description: "First copy finished but user folders are missing on the new PC? Learn how to confirm which folders were actually copied and restore the expected files."
seo_title: "Files Missing After PC Transfer: Verify User Folder Coverage"
seo_description: "First copy finished but user folders are missing on the new PC? Learn how to confirm which folders were actually copied and restore the expected files."
keywords:
  - "files missing after pc transfer"
date: 2026-11-25T09:00:08+08:00
publishDate: 2026-11-25T09:00:08+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You finished the first copy from your old Windows PC to the new one, but when you open File Explorer, your Desktop, Documents, or Pictures folders are missing or empty. This usually means the copy job skipped user folders rather than failed outright. Here is how to confirm coverage before you recopy anything.

## Check what the copy actually included

On the new PC, open File Explorer and navigate to C:\Users. You should see a folder named after your old account. Open it and compare the subfolders against the source. If Desktop, Documents, Downloads, Pictures, Music, and Videos are absent, the copy likely ran at the drive root or used a profile path that excluded user data. If the folders exist but are empty, the copy may have stopped before reaching them. Note exactly which folders are missing and whether they are absent or empty.

## Confirm the source path and copy scope

On the old PC, right-click each user folder and check Properties > Location. If the Location tab points to another drive, such as D:\Users\YourName\Documents, a copy of C:\Users alone would miss those files. This is a common cause of **files missing after pc transfer**. Record every redirected folder path and include those locations in the next copy. Also confirm the copy tool was set to include hidden items if you expect AppData or similar folders.

## Verification test

Create a small test file on the old PC inside Documents, then copy that folder again to the new PC using the corrected path. If the test file appears, your copy scope is now correct and you can proceed with the full set. If it does not, stop and check the tool's folder selection settings.

## Rollback and recovery note

Do not delete anything from the old PC until the new copy is verified. If the first copy overwrote or merged folders, restore from a backup or File History before retrying. For help confirming your specific folder layout,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
