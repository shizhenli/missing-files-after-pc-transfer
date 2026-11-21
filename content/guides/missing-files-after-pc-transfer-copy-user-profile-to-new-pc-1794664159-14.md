---
title: "Copy User Profile to New PC: Why Desktop, Documents, and AppData Are Missing"
description: "Desktop, Documents, or AppData folders missing after a Windows PC-to-PC migration? Follow these checks to diagnose an incomplete copy and restore your user profile folders."
seo_title: "Copy User Profile to New PC: Fix Missing Desktop, Documents, AppData Folders"
seo_description: "Desktop, Documents, or AppData folders missing after a Windows PC-to-PC migration? Follow these checks to diagnose an incomplete copy and restore your user profile folders."
keywords:
  - "copy user profile to new pc"
date: 2026-11-21T14:37:04+08:00
publishDate: 2026-11-21T14:37:04+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your profile to a new PC, but Desktop, Documents, or AppData folders are missing, and you want to restore the expected migration outcome before doing anything else.

## Check the source profile path first

On the old PC, open File Explorer and go to C:\Users. Confirm the exact folder name for your account (for example, C:\Users\Alex). If that folder is empty or shows only a few items, the copy never had the data. If it contains Desktop, Documents, and AppData, the source is intact and the problem is in the transfer step.

## Verify what actually arrived on the new PC

On the new PC, open C:\Users and compare folder names. A common cause is that Windows created a fresh profile (such as C:\Users\Alex.PC-NAME) while your files were copied into a different folder. Check both locations. Also enable hidden items in File Explorer's View tab, because AppData is hidden by default and may be present but invisible. If the folders exist under the wrong profile name, that explains the missing items.

## Run a verification test

Create a small test file on the old PC's Desktop, then copy the entire C:\Users\Alex folder to an external drive. On the new PC, open the copied folder and confirm the test file appears inside Desktop. If it does, your copy method works and the earlier attempt was incomplete or pointed at the wrong source.

## Recovery note

Do not delete the new profile until you confirm the old data is readable. If files were overwritten, restore them from the external drive copy or a backup before making further changes.

When you are ready to **copy user profile to new pc** correctly, map the source profile to the matching destination folder and recheck hidden items. If the folders still do not appear,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before repeating the transfer.
