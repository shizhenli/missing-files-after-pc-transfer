---
title: "External Drive Copy Incomplete: Why File Counts Don't Match and How to Fix It"
description: "External drive shows fewer files than the source after a PC-to-PC transfer? Diagnose an incomplete copy with file counts, hidden items, and a verification test."
seo_title: "External Drive Files Missing After Transfer: Fix Incomplete Copy"
seo_description: "External drive shows fewer files than the source after a PC-to-PC transfer? Diagnose an incomplete copy with file counts, hidden items, and a verification test."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-16T11:00:07+08:00
publishDate: 2026-11-16T11:00:07+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to an external drive during a PC-to-PC migration, but the drive now shows fewer files than the source. This points to an incomplete copy, not necessarily lost data.

## Check the file count and hidden items first
Open the source user folder (for example, C:\Users\YourName\Documents), right-click it, choose Properties, and note the total file count. Do the same on the external drive copy. A lower count on the drive confirms the copy stopped early. Next, in File Explorer on the drive, enable View > Show > Hidden items. If hidden files appear, the copy may have skipped system or protected files rather than user data.

## Look for partial folders and error logs
Browse the drive copy for folders that contain fewer subfolders than the source. An empty or truncated folder usually means the transfer was interrupted. If you used a copy tool, check its log or history for skipped files, access-denied errors, or a cancelled job.

## Verification test
Create a small test folder in the source Documents with three text files. Copy it to the drive using the same method. If all three files arrive, the method works and the earlier copy was interrupted. If any are missing, the method itself is skipping files.

## Recovery and rollback
Do not delete the source folders. Re-run the copy with a tool that reports errors, or copy in smaller batches. If the drive copy is incomplete, treat it as partial and recopy from the intact source. For persistent **external drive files missing after transfer** cases, stop overwriting the drive and seek guided diagnosis before making further changes.

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) if the count still does not match after a clean recopy.
