---
title: "Files Missing After PC Transfer: Fixing a Copy That Skips User Folders"
description: "A practical Windows fix for when the first PC-to-PC copy finishes but user folders or files are absent on the new PC. Check copy scope, verify with a test file, and recover safely."
seo_title: "Files Missing After PC Transfer: Fix a Copy That Skips User Folders"
seo_description: "A practical Windows fix for when the first PC-to-PC copy finishes but user folders or files are absent on the new PC. Check copy scope, verify with a test file, and recover safely."
keywords:
  - "files missing after pc transfer"
date: 2026-11-15T18:37:43+08:00
publishDate: 2026-11-15T18:37:43+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to the new Windows PC, the progress bar finished, but Desktop, Documents, or Downloads are missing on the destination.

## Check what the copy actually included

Open the destination path you used, usually C:\\Users\\<yourname>. Compare it with the source at the same path on the old PC. If the folder exists but is empty, the copy likely selected the parent folder without its contents, or skipped hidden and system items. In File Explorer, enable View > Show > Hidden items on both PCs and compare again. If the source folder shows files and the destination does not, the copy scope was wrong, not the drive.

## Confirm the source is intact

On the old PC, right-click the user folder, choose Properties, and note the size and item count. Then check the destination folder's Properties. A destination count of zero or a few kilobytes against a source of gigabytes confirms an incomplete copy. Do not delete anything on the old PC yet.

## Run a verification test

Create a small test file on the old PC's Desktop, copy it manually to the new PC's Desktop, and confirm it appears. If the test file arrives but the rest did not, the original copy excluded existing content. Re-copy each user folder individually rather than the whole Users directory.

## Rollback and recovery

Keep the old PC unchanged until the new one is verified. If **files missing after pc transfer** persist after re-copying, stop overwriting and preserve the source drive as-is. For a guided diagnosis of your exact folder layout,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
