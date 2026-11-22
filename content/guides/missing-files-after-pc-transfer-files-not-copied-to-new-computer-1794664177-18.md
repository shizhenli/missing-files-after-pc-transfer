---
title: "Why Files Are Not Copied to the New Computer After the First Copy Completes"
description: "The first copy finishes but user folders are missing on the new PC. Learn how to check the copy scope, verify folder contents, and recover from an incomplete migration."
seo_title: "Files Not Copied to New Computer: Fix the Empty User Folder"
seo_description: "The first copy finishes but user folders are missing on the new PC. Learn how to check the copy scope, verify folder contents, and recover from an incomplete migration."
keywords:
  - "files not copied to new computer"
date: 2026-11-22T10:00:09+08:00
publishDate: 2026-11-22T10:00:09+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

**files not copied to new computer**. You copied your user folders to the new PC, the progress bar finished, but Desktop, Documents, and other files are not there.

## Check the copy source and scope

Open File Explorer on the new PC and navigate to the destination folder you used (for example, C:\Users\YourName). Confirm whether the folder exists but is empty, or whether it was never created. If the folder is empty, the copy likely addressed only the parent folder and skipped its contents. If it is absent, the copy may have targeted a different drive or profile path.

On the old PC, right-click each user folder, choose Properties, and note the item count. Compare that number with what you see on the new PC. A large mismatch means the transfer did not include subfolders.

## Run a verification test

Create a small test file on the old PC inside Documents. Copy that single file to the same destination on the new PC. If it appears, the path is correct and the earlier job simply skipped nested content. If it does not appear, the destination path is wrong or permissions are blocking the write.

## Recover and retry

Do not delete the source. Re-run the copy using a method that includes subfolders, such as dragging the folder itself rather than its contents, or using robocopy with the /E switch. After the retry, recheck the item counts. If files are still not copied to new computer destinations, stop and inspect permissions on the destination profile before repeating the job.

If the counts still do not match,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before making further changes.
