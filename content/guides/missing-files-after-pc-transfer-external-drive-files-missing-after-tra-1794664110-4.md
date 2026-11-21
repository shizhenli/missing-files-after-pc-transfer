---
title: "External Drive Copy Incomplete: Why Files Are Missing After Transfer"
description: "External drive shows fewer files than the source after a PC-to-PC transfer? Diagnose an incomplete copy with folder counts, a checksum test, and a safe re-copy."
seo_title: "External Drive Files Missing After Transfer: Fix an Incomplete Copy"
seo_description: "External drive shows fewer files than the source after a PC-to-PC transfer? Diagnose an incomplete copy with folder counts, a checksum test, and a safe re-copy."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-21T14:30:50+08:00
publishDate: 2026-11-21T14:30:50+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to an external drive during a PC-to-PC migration, and now the drive shows fewer files than the source.

## Confirm the gap before changing anything
Open the source folder and the matching folder on the external drive in two File Explorer windows. Right-click each folder, choose Properties, and compare the file count and total size. A lower count on the drive means the copy stopped early. If the source is lower, the source itself may be incomplete and you should check it first.

## Check for hidden and system files
In File Explorer, enable hidden items and protected operating system files, then recount. If the numbers now match, nothing is missing; the files were simply hidden. If the drive is still short, continue.

## Look for interrupted-copy signs
Check the drive's free space. A full drive stops a copy silently. Look for leftover temporary files or folders with partial names, which indicate the transfer was cut off. Also confirm the drive is formatted with enough capacity for the full source size.

## Run a verification test
Copy one small subfolder again to a new folder on the drive and compare counts. If it matches, the original copy was interrupted, not the drive failing. If it also comes up short, test the drive on another USB port or cable before trusting it.

## Recovery and rollback
Do not delete the source folders until the drive matches. Re-copy the missing folders in smaller batches, verifying each one. If you already removed files from the old PC, stop and recover from that machine or a backup before overwriting anything.

If the drive still shows fewer files after a clean re-copy, the **external drive files missing after transfer** pattern points to a failing drive or a permissions issue.

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before formatting or erasing the drive.
