---
title: "Windows Migration Missing Folders: Why Your User Profile Folders Disappear"
description: "Desktop, Documents, or AppData folders missing after a Windows PC-to-PC migration? Follow these checks to diagnose and restore your user profile folders."
seo_title: "Windows Migration Missing Folders: Fix Missing User Profile Folders"
seo_description: "Desktop, Documents, or AppData folders missing after a Windows PC-to-PC migration? Follow these checks to diagnose and restore your user profile folders."
keywords:
  - "windows migration missing folders"
date: 2026-11-23T11:00:12+08:00
publishDate: 2026-11-23T11:00:12+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

**windows migration missing folders**. You finished a PC-to-PC migration, but now your Desktop, Documents, or AppData folders are missing from the new computer.

## Check the source profile path first

On the old PC, open File Explorer and navigate to C:\Users. Confirm the exact folder name for your user profile. It may not match your display name. Then check the new PC's C:\Users folder. If the folder exists but appears empty, the copy likely skipped hidden items. In File Explorer, enable View > Show > Hidden items and check again. If the folder is absent entirely, the migration tool did not create the profile.

## Verify folder redirection and OneDrive

On the new PC, right-click Desktop or Documents and choose Properties > Location. If the path points to a OneDrive folder, your files may be there but not where you expect. Open OneDrive settings and check backup status. If OneDrive was not signed in, the folders may still exist locally under C:\Users\<name>\OneDrive.

## Run a verification test

Create a test file on the old PC's Desktop, then copy it manually to the new PC's Desktop. If it appears, the folder structure is intact and only the bulk copy failed. If it does not appear, the profile folder is missing or redirected.

## Rollback and recovery

Before making changes, create a restore point. If the migration overwrote or removed folders, recover them from the old PC's drive or a backup. Do not delete the new profile until you confirm the data is safe.

If these checks do not restore your folders, the migration likely missed user profile folders due to permissions or hidden-file handling.

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) for a guided diagnosis.
