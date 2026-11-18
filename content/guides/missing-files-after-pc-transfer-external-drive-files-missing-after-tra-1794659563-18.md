---
title: "External Drive Shows Fewer Files Than the Source After Transfer: Fixing an Incomplete Copy"
description: "External drive shows fewer files than the source after a PC-to-PC transfer? Follow these checks to diagnose an incomplete copy and recover missing files safely."
seo_title: "External Drive Files Missing After Transfer: Fix an Incomplete Copy"
seo_description: "External drive shows fewer files than the source after a PC-to-PC transfer? Follow these checks to diagnose an incomplete copy and recover missing files safely."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-18T12:00:19+08:00
publishDate: 2026-11-18T12:00:19+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to an external drive during a PC-to-PC migration, but the drive now shows fewer files than the source.

## Confirm the copy is actually incomplete

First, compare counts without trusting the file explorer. On the source PC, open Command Prompt and run `robocopy "C:\Users\YourName\Documents" "E:\Backup\Documents" /L /E /NJH /NJS /FP /NS /NC`. The `/L` switch lists what would be copied without changing anything. If the output shows files that are absent on the external drive, the copy is incomplete rather than a display glitch.

Next, check hidden items. In File Explorer, enable hidden items and protected operating system files. If folders such as AppData now appear, the files were copied but hidden. If they remain absent, continue.

## Check for path length and permission failures

Long paths often stop a copy silently. Compare the deepest folder paths on both sides; any source path beyond roughly 260 characters is a likely failure point. Also confirm your account has read access to every source folder. A folder that denied access during the copy will be missing on the drive even though the transfer reported no error.

## Verification test

Create a small test folder on the source with three files, copy it to the external drive, and confirm all three arrive. Then copy one previously missing folder and recheck its file count. If the test succeeds but the original folder still fails, the problem is specific to that folder's path or permissions, not the drive.

## Rollback and recovery

Do not delete anything from the source PC. Reconnect the drive, rerun the copy with `robocopy` using `/E /COPY:DAT /R:1 /W:1`, and log the output with `/LOG+:copy.log` so failures are recorded. Keep the source intact until the drive's file count matches.

If the **external drive files missing after transfer** persist after these checks,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before reformatting or overwriting the drive.
