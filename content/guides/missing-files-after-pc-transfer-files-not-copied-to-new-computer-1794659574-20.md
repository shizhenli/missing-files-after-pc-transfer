---
title: "Files Not Copied to New Computer: Fixing a Copy That Skips User Folders"
description: "Your first copy finished, but user folders are absent on the new PC. Follow these checks to diagnose why files not copied to new computer and restore them."
seo_title: "Files Not Copied to New Computer: Fix a Copy That Skips User Folders"
seo_description: "Your first copy finished, but user folders are absent on the new PC. Follow these checks to diagnose why files not copied to new computer and restore them."
keywords:
  - "files not copied to new computer"
date: 2026-11-21T14:30:50+08:00
publishDate: 2026-11-21T14:30:50+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You ran a PC-to-PC transfer, the progress bar completed, but your user folders are missing on the new computer. Here is how to diagnose that specific failure before you recopy anything.

## Check the source path and hidden items

On the old PC, open File Explorer and navigate to C:\Users. Confirm your profile folder exists and is not just a shortcut. Then enable View > Hidden items. If your Desktop, Documents, or Downloads folders appear faded, they are hidden and may have been skipped by a copy that ignored hidden files. Result to interpret: visible folders with content mean the source is intact; empty or shortcut-only folders mean the copy had nothing to transfer.

## Check the copy method and destination

On the new PC, open C:\Users and compare folder names. If your old profile folder is absent but a folder like C:\Users\YourName.000 exists, Windows created a temporary profile during setup and the copy landed elsewhere. Search the new drive for one known filename from Documents. If it appears under a different path, the transfer completed but not to the expected profile. This is the common reason **files not copied to new computer** appear missing.

## Verification test

Create a test file named transfer-check.txt in the old PC's Documents folder, copy it manually to the new PC's Documents folder, and confirm it opens. If the manual copy works but the bulk transfer did not, the original tool skipped user folders.

## Rollback and recovery

Do not delete the old PC's data. If the destination profile is wrong, copy the missing folders into the correct C:\Users profile, then sign out and back in to confirm they appear. If the source folders were hidden, recopy with hidden items enabled. For a guided diagnosis,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
