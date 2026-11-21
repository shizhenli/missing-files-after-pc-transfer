---
title: "Windows Migration Missing Folders: Why Desktop, Documents, and AppData Disappear"
description: "Fix windows migration missing folders after a PC-to-PC transfer. Check profile paths, verify hidden folders, and restore Desktop, Documents, and AppData safely."
seo_title: "Windows Migration Missing Folders: Restore Desktop, Documents, and AppData"
seo_description: "Fix windows migration missing folders after a PC-to-PC transfer. Check profile paths, verify hidden folders, and restore Desktop, Documents, and AppData safely."
keywords:
  - "windows migration missing folders"
date: 2026-11-21T14:33:58+08:00
publishDate: 2026-11-21T14:33:58+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You finished a Windows PC-to-PC migration, but now Desktop, Documents, or AppData folders are missing from your user profile. This points to a path or copy-scope issue, not lost data.

## Check the actual profile path first
Open File Explorer and paste `%USERPROFILE%` into the address bar. Press Enter. You should land in `C:\Users\<yourname>`. If you land in a different folder, or if Desktop and Documents are absent, the migration may have created a new profile instead of copying the old one. Look for a second folder under `C:\Users` with your old account name. If it exists, your files are likely there.

## Verify hidden and system folders
AppData is hidden by default. In File Explorer, open View > Show > Hidden items. Then navigate to `C:\Users\<yourname>\AppData`. If AppData is still missing, the migration tool skipped hidden folders. Check `C:\Users\<oldname>\AppData` as well. If both are empty, the copy scope excluded system files.

## Run a verification test
Create a test file on the old PC's Desktop, then copy it manually to the new PC's Desktop. If it appears, the folder structure is intact and only the automated migration missed it. If it does not appear, confirm you are copying to the correct user profile.

## Rollback and recovery note
Before making changes, do not delete the old profile folder. If the migration created a duplicate profile, sign in with the old account or copy missing folders from `C:\Users\<oldname>` into the new profile. Keep a backup of AppData before merging, as overwriting can break applications.

If these checks show the folders were never copied, this is a common case of **windows migration missing folders** and can be resolved by recopying the specific profile directories. For guided recovery,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
