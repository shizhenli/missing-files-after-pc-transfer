---
title: "User Folders Empty After First Copy: Diagnosing Missing Files on the New PC"
description: "First copy finished but user folders are empty on the new PC? Follow these checks to diagnose missing files after PC transfer and recover your data safely."
seo_title: "Files Missing After PC Transfer: Fix Empty User Folders"
seo_description: "First copy finished but user folders are empty on the new PC? Follow these checks to diagnose missing files after PC transfer and recover your data safely."
keywords:
  - "files missing after pc transfer"
date: 2026-11-24T09:00:09+08:00
publishDate: 2026-11-24T09:00:09+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

**files missing after pc transfer**. You copied your user folders to the new PC, but Desktop, Documents, or Downloads are empty or incomplete.

## Confirm what actually copied
Open File Explorer on the new PC and navigate to C:\Users\<your-username>. Compare folder names against the old PC. If the folder exists but is empty, the copy likely skipped hidden or permission-protected content. If the folder is absent entirely, the transfer targeted a different profile path. Right-click each folder, choose Properties, and note the size and item count. A size of 0 bytes or a count far below the source confirms an incomplete copy, not a deletion.

## Check hidden items and profile path
In File Explorer, enable View > Show > Hidden items. Many user files live in AppData, which is hidden by default. If AppData is missing, the copy tool excluded it. Also verify you are looking at the correct profile: C:\Users\<name> versus C:\Users\<name>.old or a temp migration folder. A mismatch here explains why user folders appear absent even though data exists elsewhere on disk.

## Verification test
Create a test file on the old PC inside Documents, then copy that single file to the same path on the new PC. If it lands correctly, the path and permissions are fine and the original bulk copy was incomplete. If it fails, permissions or the destination profile are the problem.

## Recovery and rollback
Do not delete the old PC data or any migration temp folder until verified. Re-run the copy with a tool that preserves hidden files and permissions, or copy AppData separately. If files are missing after pc transfer and the source is still intact, restore from the original drive rather than guessing. For guided diagnosis,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
