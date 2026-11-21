---
title: "Files Not Copied to New Computer: Fixing a First Copy That Leaves User Folders Empty"
description: "First copy finishes but user folders are empty on the new PC? Check source paths, hidden folders, and copy method, then verify with a test file and recover safely."
seo_title: "Files Not Copied to New Computer: Fix Empty User Folders After First Copy"
seo_description: "First copy finishes but user folders are empty on the new PC? Check source paths, hidden folders, and copy method, then verify with a test file and recover safely."
keywords:
  - "files not copied to new computer"
date: 2026-11-21T14:37:04+08:00
publishDate: 2026-11-21T14:37:04+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to the new PC, the progress bar finished, but Desktop, Documents, and similar folders are empty on the destination.

## Check what the first copy actually included
On the old PC, open File Explorer and navigate to C:\Users\<your-name>. Confirm the folders you expect (Desktop, Documents, Downloads, Pictures) are visible. If they are not, enable View > Show > Hidden items. Then right-click each folder, choose Properties, and note the exact path under Location. A common cause is that the copy job pointed at the profile root or a library shortcut rather than the real folder path. If the source path shown differs from what you selected in the copy tool, that explains why **files not copied to new computer**.

## Confirm the destination and copy method
On the new PC, open the destination folder and check the address bar. If you copied into a parent folder, the files may be one level deeper than expected. Also check whether the copy completed as a move or merge that skipped existing folders. Compare item counts: right-click the source folder, Properties, and note the number of files; do the same on the destination. A large mismatch means the copy did not traverse subfolders.

## Verification test
Create a small test file on the old PC inside Documents, named test-copy.txt. Copy that single file to the new PC's Documents folder. If it appears, the copy path works and the earlier job likely missed subfolders. If it does not appear, the destination is wrong or permissions are blocking writes.

## Rollback and recovery
Do not delete anything on the old PC until the new copy is verified. If the first copy overwrote or merged folders, restore from a backup or previous version before retrying. For a controlled diagnosis,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
