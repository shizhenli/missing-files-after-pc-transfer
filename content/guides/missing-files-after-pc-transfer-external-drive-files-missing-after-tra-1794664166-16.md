---
title: "External Drive Copy Incomplete: Verifying and Recovering Missing Files"
description: "External drive shows fewer files than the source after a PC-to-PC transfer? Follow these checks to confirm an incomplete copy and recover your data safely."
seo_title: "External Drive Files Missing After Transfer: Fix an Incomplete Copy"
seo_description: "External drive shows fewer files than the source after a PC-to-PC transfer? Follow these checks to confirm an incomplete copy and recover your data safely."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-22T08:00:10+08:00
publishDate: 2026-11-22T08:00:10+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to an external drive during a PC-to-PC migration, but the drive now shows fewer files than the source.

## Confirm the copy is actually incomplete

First, compare counts without trusting the folder view. In File Explorer, open the source user folder, right-click it, choose Properties, and note the total file count. Do the same on the external drive copy. A lower count on the drive confirms an incomplete copy rather than a display glitch. Next, enable hidden items (View > Show > Hidden items) on both sides. If the source shows more hidden files, the copy likely skipped them.

## Check for common causes

Look at the drive's free space. If it is nearly full, the copy stopped early. Check the transfer log or any error dialog you dismissed; access-denied or path-too-long errors are common with user folders. Also verify you copied the folder contents, not just the folder shell, and that no sync tool is still running in the background.

## Run a verification test

Create a small test folder in the source Documents with three files, copy it to the external drive, and confirm all three appear. If they do, the connection and permissions are working; if not, the drive or cable is the problem. This tells you whether to retry the copy or replace the hardware.

## Recover and roll back safely

Do not delete the source until the copy is verified. Re-run the copy with a tool that reports errors, such as robocopy in a command prompt, and review its summary for skipped files. If files are still missing, treat the **external drive files missing after transfer** as a signal to stop and diagnose before overwriting anything. Keep the original source intact as your rollback point.

If the counts still do not match after a clean retry,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before making further changes.
