---
title: "External Drive Files Missing After Transfer: Diagnosing an Incomplete Copy"
description: "External drive shows fewer files than the source after a PC-to-PC transfer? Diagnose an incomplete copy with checks, a verification test, and recovery steps."
seo_title: "External Drive Files Missing After Transfer: Fix Incomplete Copy"
seo_description: "External drive shows fewer files than the source after a PC-to-PC transfer? Diagnose an incomplete copy with checks, a verification test, and recovery steps."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-15T18:37:43+08:00
publishDate: 2026-11-15T18:37:43+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to an external drive during a PC-to-PC migration, but the drive now shows fewer files than the source.

## Confirm the copy actually finished

Open File Explorer, right-click the external drive, and choose Properties. Compare the total size and file count against the source folder. A large gap means the copy stopped early. If the drive shows nearly full, the destination ran out of space mid-transfer. Free space or use a larger drive, then recopy the missing folders.

Next, check for hidden items. In File Explorer, open View and enable Hidden items. If folders like AppData or Desktop appear now, they were copied but hidden. That is not data loss.

## Check for skipped or locked files

Review the copy log if your migration tool produced one. Look for skipped files, access-denied errors, or long paths. Files open in another program are often skipped silently. Close all applications, then recopy only the affected folders.

## Verification test

Pick one missing folder, such as Documents. Compare its file count and size on the source and the external drive using Properties. They should match. Then open two or three files from the drive to confirm they are readable, not zero-byte placeholders.

## Recovery note

Do not format or write new data to the external drive until you finish checking. If files are still absent, recopy from the original PC while it is still available. If the source is gone, stop using the drive and seek recovery advice before making changes. For a guided diagnosis of your **external drive files missing after transfer**,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
