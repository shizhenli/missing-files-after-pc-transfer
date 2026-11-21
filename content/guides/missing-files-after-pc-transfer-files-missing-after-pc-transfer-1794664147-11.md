---
title: "User Folders Absent on the New PC After the First Copy: Diagnosing a Transfer That Reports Success but Leaves Nothing"
description: "First copy finishes but user folders are absent on the new PC. Step-by-step checks to confirm whether the transfer skipped your profile, plus a verification test and rollback note."
seo_title: "Files Missing After PC Transfer: Fix the Empty User Folders"
seo_description: "First copy finishes but user folders are absent on the new PC. Step-by-step checks to confirm whether the transfer skipped your profile, plus a verification test and rollback note."
keywords:
  - "files missing after pc transfer"
date: 2026-11-21T14:37:04+08:00
publishDate: 2026-11-21T14:37:04+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to the new PC, the progress bar finished, but Desktop, Documents, and Pictures are nowhere on the destination drive.

## Confirm what the copy actually wrote

Open File Explorer on the new PC and navigate to the destination path you selected. Check the folder properties: right-click the destination folder, choose Properties, and read the size and file count. If the size is a few kilobytes or the count is zero, the copy created the folder shell but never wrote the contents. That is the signature of a skipped source or an aborted job, not a deletion.

Next, compare against the source. On the old PC, open the same user folder and note the item count. A large gap between source and destination confirms an incomplete transfer rather than a display glitch.

## Check whether the profile was redirected

On the new PC, open Settings > System > Storage > Advanced storage settings and review where new content saves. If OneDrive or another sync client took over Desktop, Documents, and Pictures, the files may sit under a cloud path instead of C:\Users\YourName. Sign in to the sync client and look for the folders there before assuming data loss.

## Verification test

Create a small test file on the old PC inside Documents, copy it manually to the same destination path on the new PC, and confirm it appears. If the manual copy succeeds where the bulk job failed, the original transfer skipped that folder and a targeted re-copy is safe.

## Rollback and recovery

Do not delete anything on the old PC until the new copy is verified. If the source folder is now empty, check the Recycle Bin and any backup or File History drive before re-running the transfer. These **files missing after pc transfer** cases usually resolve once the skipped folder is copied directly.

If the destination stays empty after a manual copy, stop and

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before making further changes.
