---
title: "Copy User Profile to New PC: When Desktop, Documents, and AppData Are Missing After Migration"
description: "Fix a Windows PC-to-PC migration that misses user profile folders. Check profile paths, verify folder presence, and recover missing Desktop, Documents, and AppData."
seo_title: "Copy User Profile to New PC: Fix Missing Desktop, Documents, AppData"
seo_description: "Fix a Windows PC-to-PC migration that misses user profile folders. Check profile paths, verify folder presence, and recover missing Desktop, Documents, and AppData."
keywords:
  - "copy user profile to new pc"
date: 2026-11-21T14:33:58+08:00
publishDate: 2026-11-21T14:33:58+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

**copy user profile to new pc**. You copied your user profile to a new PC, but after migration the Desktop, Documents, or AppData folders are not present. This usually means the copy targeted the wrong profile path or skipped hidden folders, not that the data is gone.

## Check the actual profile path
On the new PC, open File Explorer and paste %USERPROFILE% into the address bar. Press Enter. You should land in C:\Users\YourName. If the folder name differs from the old PC (for example, YourName vs YourName.000), the migration copied into a different profile. That mismatch explains why folders appear missing.

## Verify folder presence and hidden items
In File Explorer, enable View > Show > Hidden items. Then check for Desktop, Documents, and AppData inside %USERPROFILE%. If AppData is still absent, confirm you copied from the old PC's C:\Users\OldName\AppData, not from a parent folder. A common mistake is copying C:\Users\OldName without including the hidden AppData subfolder.

## Run a verification test
Create a test file on the old PC's Desktop named migration-test.txt. Copy it again using the same method. On the new PC, search for migration-test.txt. If it appears under a different user folder, your copy destination was wrong. If it does not appear at all, the source selection missed the folder.

## Rollback and recovery note
Before overwriting anything, rename the new profile's existing Desktop and Documents folders to Desktop_old and Documents_old. Then re-copy the correct folders from the old profile. If the old PC is still available, keep it unchanged until you confirm the new PC shows all expected folders.

If these checks do not restore the folders, stop repeating the same copy.

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) so the profile path and copy scope can be diagnosed before you risk overwriting data.
