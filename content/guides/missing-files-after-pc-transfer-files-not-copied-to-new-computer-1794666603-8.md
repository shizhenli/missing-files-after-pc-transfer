---
title: "Files Not Copied to New Computer: When the First Copy Leaves User Folders Empty"
description: "First copy finished but user folders are empty on the new PC? Follow these checks to confirm whether files not copied to new computer and restore your data safely."
seo_title: "Files Not Copied to New Computer: Fix Empty User Folders"
seo_description: "First copy finished but user folders are empty on the new PC? Follow these checks to confirm whether files not copied to new computer and restore your data safely."
keywords:
  - "files not copied to new computer"
date: 2026-11-24T10:00:05+08:00
publishDate: 2026-11-24T10:00:05+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to the new PC, but when you open File Explorer, Desktop, Documents, and Pictures are empty or missing.

## Check what actually copied

Open File Explorer on the new PC and navigate to C:\Users\<your-username>. Compare the folder list with the old PC. If the folders exist but are empty, the copy likely skipped hidden or permission-protected content. If the folders are absent entirely, the copy targeted a different profile path or a temporary folder.

Right-click each expected folder, choose Properties, and read the Size and Contains values. A size of 0 bytes or a missing folder confirms the data did not land there.

## Confirm the source and destination

On the old PC, verify the exact path of your user folders. On the new PC, check whether the copy created a nested folder such as C:\Users\<your-username>\Desktop\Desktop. If so, the files are present but one level deeper than expected. Move them up one level and retest.

## Run a verification test

Create a small test file on the old PC Desktop, copy it to the new PC Desktop, and confirm it appears. Then repeat with a file from Documents. If the test file copies but your original files do not, the issue is with hidden items or access permissions, not the transfer method. This is the point where most people realize **files not copied to new computer** because the copy tool skipped protected folders.

## Rollback and recovery

Do not delete anything from the old PC until the new PC shows the expected files. If the copy is incomplete, recopy the missing folders directly from the old PC to an external drive first, then to the new PC. If folders remain empty after a direct copy, stop and

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before making further changes.
