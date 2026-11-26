---
title: "External Drive Files Missing After Transfer: Confirming and Fixing an Incomplete Copy"
description: "External drive shows fewer files than the source after a PC-to-PC transfer? Confirm the copy is incomplete, re-run it safely, and verify the result."
seo_title: "External Drive Files Missing After Transfer: Fix the Incomplete Copy"
seo_description: "External drive shows fewer files than the source after a PC-to-PC transfer? Confirm the copy is incomplete, re-run it safely, and verify the result."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-26T08:59:17+08:00
publishDate: 2026-11-26T08:59:17+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to an external drive during a PC-to-PC move, and now the drive shows fewer files than the source.

## Confirm the copy is actually incomplete

Open the source folder and the matching folder on the external drive side by side. In File Explorer, right-click each folder, choose Properties, and compare the item count and total size. A lower count on the drive means the copy stopped early. Then check the drive itself: open This PC, right-click the external drive, and look at free space. If free space is far larger than expected, files were never written. Also look for a folder named the same as the source with a suffix such as (1) or - Copy; Windows sometimes redirects a second copy there.

## Find out why it stopped

Reconnect the drive to a different USB port, preferably one directly on the PC rather than a hub. In Event Viewer, open Windows Logs and check System for disk or USB errors around the transfer time. If the drive is formatted FAT32, a single file over 4 GB will fail silently; confirm the file system under Properties. A drive that disconnects mid-copy is the most common cause of **external drive files missing after transfer**.

## Re-run the copy safely

Do not delete anything on the source. Create a new folder on the drive, then copy one user folder at a time rather than the whole set. After each folder, compare Properties counts again. If a folder fails twice, note the exact file where it stops.

## Verification test

Copy a small test folder, eject the drive properly, reconnect it, and confirm the test files open. Then repeat the count comparison on the folders you already copied.

## Rollback note

Keep the source folders untouched until the drive matches them. If a re-copy creates duplicates, remove only the newly created duplicate folder, never the original.

If the count still falls short,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before deleting anything.
