---
title: "Windows Migration Missing Folders: Recovering Your User Profile Folders"
description: "After a Windows PC-to-PC migration, your Desktop, Documents, or AppData folders are missing. Follow these steps to diagnose and recover your user profile folders."
seo_title: "Windows Migration Missing Folders: Fix Missing Desktop, Documents, AppData"
seo_description: "After a Windows PC-to-PC migration, your Desktop, Documents, or AppData folders are missing. Follow these steps to diagnose and recover your user profile folders."
keywords:
  - "windows migration missing folders"
date: 2026-11-16T08:00:07+08:00
publishDate: 2026-11-16T08:00:07+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You've migrated to a new PC, but your Desktop, Documents, or AppData folders are nowhere to be found.

## Check the Source Profile Folder

First, confirm the folders exist on the old PC. Open File Explorer and navigate to `C:\Users\<YourUsername>`. Look for Desktop, Documents, and AppData. If they're present, the issue is with the copy process, not the data itself. If they're missing there, check if OneDrive has redirected them: right-click each folder, choose Properties, and see if the Location tab points to a OneDrive path.

## Verify Hidden Folders and Permissions

On the new PC, open File Explorer, go to View, and enable Hidden items. AppData is hidden by default, so it may be there but invisible. Also, check that you're signed in with the same account name. If the migration created a new profile (e.g., `Username_2`), your old folders may be under the original profile folder.

## Run a Verification Test

Create a test file on the old PC's Desktop, then manually copy it to the new PC's Desktop. If it appears, basic file transfer works. If not, the migration tool may have skipped user folders due to permissions or profile conflicts. This is a common cause of **windows migration missing folders**.

## Rollback and Recovery

If folders are still missing, do not overwrite anything. Restore from your backup or use the migration tool's logs to identify skipped paths. Manually copy the missing folders from the old PC using an external drive, ensuring you include hidden items.

If you need guided help,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
