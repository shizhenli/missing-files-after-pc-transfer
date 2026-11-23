---
title: "External Drive Files Missing After Transfer: Completing an Incomplete Copy"
description: "External drive shows fewer files than the source after a PC-to-PC transfer? Learn how to diagnose and complete an incomplete copy, verify results, and recover safely."
seo_title: "External Drive Files Missing After Transfer: Fix an Incomplete Copy"
seo_description: "External drive shows fewer files than the source after a PC-to-PC transfer? Learn how to diagnose and complete an incomplete copy, verify results, and recover safely."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-23T08:00:09+08:00
publishDate: 2026-11-23T08:00:09+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to an external drive during a PC-to-PC migration, but now the drive shows fewer files than the source.

## Confirm the copy is actually incomplete

First, compare counts. In File Explorer, open the source user folder and the matching folder on the external drive. Right-click each folder, choose Properties, and note the number of files and total size. If the external drive's count or size is lower, the copy is incomplete. If they match but files appear missing, the issue may be hidden items or a display filter—check View > Show > Hidden items.

Next, check free space on the external drive. If it is nearly full, the copy likely stopped early. Also review the transfer log or any error dialog you dismissed; a single failed file can halt a bulk copy.

## Run a verification test

Create a small test folder on the source with a few files, copy it to the external drive, and confirm all files appear. Then copy one previously missing subfolder again. If it completes and the count rises, the original transfer was interrupted rather than the files being lost.

## Complete the copy and recover safely

Re-run the copy for only the missing folders using a tool that reports errors, such as robocopy with logging. Do not delete anything from the source until the external drive count matches. If files still will not copy, note the exact error and stop—this is your rollback point. Keep the source untouched as your recovery copy.

For a controlled diagnosis of why the **external drive files missing after transfer**,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
