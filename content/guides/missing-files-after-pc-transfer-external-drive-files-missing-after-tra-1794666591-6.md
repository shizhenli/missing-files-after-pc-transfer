---
title: "External Drive Shows Fewer Files Than the Source: Completing an Interrupted Copy"
description: "Your external drive shows fewer files than the source after a PC-to-PC transfer. Follow these checks to diagnose and complete the interrupted copy, with a rollback note."
seo_title: "External Drive Files Missing After Transfer: Fix an Incomplete Copy"
seo_description: "Your external drive shows fewer files than the source after a PC-to-PC transfer. Follow these checks to diagnose and complete the interrupted copy, with a rollback note."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-24T08:00:09+08:00
publishDate: 2026-11-24T08:00:09+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to an external drive during a PC-to-PC migration, but the drive now shows fewer files than the source.

## Confirm what actually copied

Open File Explorer, right-click the source user folder, choose Properties, and note the file count and total size. Do the same on the external drive copy. A lower count or size means the copy stopped early, which is the usual cause of **external drive files missing after transfer**.

Next, check free space on the external drive. If the copy needed more room than remained, Windows stops without a clear warning. Compare the drive's free space against the source folder size; if free space is smaller, that explains the shortfall.

## Look for a partial copy

Inspect the destination folder for a temporary file or a folder with the same name plus a suffix. A leftover partial file means the transfer was interrupted. Also check the USB cable and port: a loose connection or a power-saving USB hub can drop the drive mid-copy.

## Verification test

Create a small test folder on the source with a few files, copy it to the external drive, and confirm every file appears. Then copy one large subfolder and watch until it finishes. If the test copy completes fully, the original interruption was likely connection or space related; retry the full copy after freeing space and using a direct rear USB port.

## Rollback and recovery

Do not delete the source folders until the external copy matches in count and size. If a partial file exists on the drive, delete only that incomplete item and recopy the affected folder. Keep the source intact as your rollback point.

If the counts still differ after a clean retry,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
