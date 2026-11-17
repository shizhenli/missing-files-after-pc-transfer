---
title: "External Drive Files Missing After Transfer: Verifying the Copy Before You Reformat"
description: "External drive files missing after transfer? Check source paths, hidden files, and copy logs to confirm whether the first pass skipped your user folders, then recover safely."
seo_title: "External Drive Files Missing After Transfer: Fix the Empty Copy"
seo_description: "External drive files missing after transfer? Check source paths, hidden files, and copy logs to confirm whether the first pass skipped your user folders, then recover safely."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-17T11:00:08+08:00
publishDate: 2026-11-17T11:00:08+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to an external drive, but on the new PC the drive looks empty or only partially populated.

## Confirm the source paths actually match

Open File Explorer on the old PC and navigate to C:\Users\<yourname>. Confirm Desktop, Documents, Downloads, and Pictures exist there. If any folder shows a shortcut arrow, it is redirected to OneDrive or another location, and a plain copy of C:\Users will not include its contents. Right-click each folder, choose Properties, and read the Location field. If it points outside C:\Users, copy from that actual path instead.

## Check for hidden and system files

On the external drive, enable View > Show > Hidden items. A copy that appears empty may simply be hiding files. Also compare folder sizes: right-click the source folder, then the destination folder, and read the byte counts. A destination far smaller than the source means the copy stopped early or skipped files.

## Run a verification test

Create a small test folder on the old PC with three known files. Copy it to the external drive, eject safely, reconnect, and open it on the new PC. If the test files appear, the drive and cable are fine and the original copy was incomplete. If they do not, the drive or connection is the problem.

## Recovery note

Do not reformat the old PC or the external drive yet. Recopy the missing folders using a direct path, and keep the original data untouched until the new PC shows matching file counts. If **external drive files missing after transfer** persists after a second verified copy, stop repeating the same step.

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before making further changes.
