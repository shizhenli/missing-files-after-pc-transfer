---
title: "External Drive Files Missing After Transfer: Fixing an Incomplete Copy"
description: "External drive shows fewer files than the source after a PC-to-PC transfer? Check copy method, hidden items, and free space, then verify with a hash comparison and recover safely."
seo_title: "External Drive Files Missing After Transfer: Fix an Incomplete Copy"
seo_description: "External drive shows fewer files than the source after a PC-to-PC transfer? Check copy method, hidden items, and free space, then verify with a hash comparison and recover safely."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-17T12:00:06+08:00
publishDate: 2026-11-17T12:00:06+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to an external drive during a PC-to-PC migration, and now the drive shows fewer files than the source.

## Confirm what actually copied
Open File Explorer, right-click the source user folder, choose Properties, and note the item count and size. Do the same on the external drive copy. A lower count means the copy stopped early or skipped items. If the counts match but files appear missing, enable View > Show > Hidden items and check for folders like AppData, which is hidden by default.

## Check the copy method and space
If you used drag-and-drop, Windows may have paused on a long path or a file in use without a clear error. Re-run the copy with a tool that logs failures, such as robocopy in a Command Prompt: robocopy "C:\Users\Name" "E:\Backup\Name" /E /R:1 /W:1 /LOG:E:\copy.log. Open the log and look for ERROR lines. Also confirm the external drive has enough free space; a full drive silently truncates large folders.

## Verification test
Compare a sample: pick three subfolders, check their file counts on both sides, and open one document from each. Then run a hash check on a few files with certutil -hashfile on source and copy; matching hashes confirm the copy is intact. If hashes differ, treat the copy as incomplete.

## Rollback and recovery
Do not delete the source until verification passes. If the copy is incomplete, recopy the affected folders to a new folder on the drive rather than overwriting, so you can compare. Keep the original source untouched as your rollback point.

If the **external drive files missing after transfer** persist after a clean recopy,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before making further changes.
