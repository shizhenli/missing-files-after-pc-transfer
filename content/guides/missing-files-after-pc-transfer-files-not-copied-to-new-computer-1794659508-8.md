---
title: "Files Not Copied to New Computer: Why the First Copy Leaves User Folders Empty"
description: "First copy finished but user folders are empty on the new PC? Diagnose an incomplete transfer with exact checks, a verification test, and a safe recovery path."
seo_title: "Files Not Copied to New Computer: Fix Empty User Folders After Transfer"
seo_description: "First copy finished but user folders are empty on the new PC? Diagnose an incomplete transfer with exact checks, a verification test, and a safe recovery path."
keywords:
  - "files not copied to new computer"
date: 2026-11-17T08:00:13+08:00
publishDate: 2026-11-17T08:00:13+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to the new Windows PC, the progress bar finished, but Desktop, Documents, and other folders are empty or missing.

## Check the source and destination paths

On the old PC, open File Explorer and navigate to C:\Users\<your-username>. Confirm the folders you expect are present and contain files. On the new PC, open the same path. If the new PC shows a different username folder (for example, a Microsoft account name instead of your local name), your files may have landed in a folder you are not viewing. Compare the full paths, not just folder names.

## Interpret what you see

If the source folders are empty, the original copy never had data to move. If the destination folder exists but is empty, the copy likely skipped hidden or protected items. In File Explorer, enable View > Hidden items on both PCs. Check whether AppData and other hidden folders exist at the source. A missing AppData on the destination is expected if you copied only visible folders.

## Run a verification test

Create a small test file on the old PC inside Documents. Copy that single file to the same Documents path on the new PC. If it appears, the path is correct and the earlier copy was incomplete. If it does not appear, you are copying to the wrong user folder. This tells you whether the problem is path selection or copy scope.

## Recover without overwriting

Do not delete anything on the new PC yet. Re-copy the missing folders from the old PC into a new folder such as C:\Users\<your-username>\Recovered, then move contents into place after confirming they are complete. If the old PC is no longer available, check any external drive or backup used during the transfer before making changes.

If these checks show the **files not copied to new computer** and you need a controlled diagnosis,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
