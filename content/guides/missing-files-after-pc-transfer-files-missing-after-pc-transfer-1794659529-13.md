---
title: "Files Missing After PC Transfer: Diagnosing an Incomplete First Copy"
description: "First copy finished but user folders are missing on the new PC? Follow these checks to diagnose an incomplete transfer and recover your files."
seo_title: "Files Missing After PC Transfer: Fix an Incomplete First Copy"
seo_description: "First copy finished but user folders are missing on the new PC? Follow these checks to diagnose an incomplete transfer and recover your files."
keywords:
  - "files missing after pc transfer"
date: 2026-11-18T08:00:13+08:00
publishDate: 2026-11-18T08:00:13+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

**files missing after pc transfer**. You copied your user folders to the new PC, but when you open File Explorer, Desktop, Documents, and other folders are empty or absent—so you're stuck before you can even diagnose why files are missing after a pc transfer.

## Check the source folder first
On the old PC, open File Explorer and navigate to C:\Users\<your-username>. Right-click each user folder (Desktop, Documents, Downloads, Pictures) and choose Properties. Look at the Size and Contains values. If a folder shows 0 bytes or very few files, the source may be a redirected or OneDrive-only folder, and the copy had nothing to transfer. If sizes look normal, the issue is on the destination side.

## Inspect the destination path
On the new PC, open C:\Users\<your-username>. Confirm the folders exist and are not hidden. In File Explorer, enable View > Hidden items. Then right-click each folder and check Properties again. Compare file counts with the source. A folder that exists but is empty means the copy created the directory without transferring contents—a classic incomplete first copy.

## Run a verification test
Create a small test file on the old PC's Desktop, copy it manually to the new PC's Desktop, and confirm it appears. If that works, the connection and permissions are fine, and the original transfer simply skipped files. If it fails, check whether the destination folder is read-only or controlled by a different account.

## Rollback and recovery
Before retrying, do not delete anything on the old PC. Re-run the copy using a method that preserves folder structure, such as robocopy with /E, and verify counts again. If folders remain empty, stop and

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) so the transfer can be reviewed without risking the source data.
