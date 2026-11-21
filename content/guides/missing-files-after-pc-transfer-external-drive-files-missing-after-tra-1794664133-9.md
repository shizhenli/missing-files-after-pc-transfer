---
title: "External Drive Files Missing After Transfer: Fixing the Empty Destination"
description: "Fix external drive files missing after transfer on Windows. Check copy scope, hidden files, and verify with a test folder before recovery."
seo_title: "External Drive Files Missing After Transfer: Fix the Empty Destination"
seo_description: "Fix external drive files missing after transfer on Windows. Check copy scope, hidden files, and verify with a test folder before recovery."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-21T14:33:58+08:00
publishDate: 2026-11-21T14:33:58+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied user folders from an external drive to a new PC, but the destination looks empty.

## Confirm what the copy actually included

Open the source external drive in File Explorer. Right-click the user folder, choose Properties, and compare the size and file count with the destination folder. If the source shows 12 GB and the destination shows 0 bytes, the copy did not include the contents. Check whether you dragged the folder itself into an existing folder with the same name. Windows may have created a nested path such as Documents\Documents. Navigate one level deeper and look for your files there.

Next, enable hidden items in File Explorer View settings. User folders often contain hidden system files, and a partial copy can leave only those behind. If you see only desktop.ini or thumbs.db, the visible files were skipped.

## Run a verification test

Create a small test folder on the external drive with three known files. Copy it to the new PC using the same method you used before. If the test folder arrives complete, the original copy was interrupted or scoped incorrectly. If the test folder is also empty, the transfer method itself is dropping files.

## Recover before overwriting

Do not delete the source drive or run another full copy yet. Check the destination for a folder named after the source drive or a duplicate user folder. If the files are still missing, stop and preserve both drives as they are.

If these checks do not explain the gap, the issue may be a permissions or profile-path problem.

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before making further changes. For **external drive files missing after transfer**, confirming the exact destination path is the fastest way to avoid a second failed copy.
