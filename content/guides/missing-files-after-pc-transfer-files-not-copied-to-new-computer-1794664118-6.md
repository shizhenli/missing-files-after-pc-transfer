---
title: "Files Not Copied to New Computer: Verifying the First Copy and Recovering Missing User Folders"
description: "First copy finished but user folders are missing on the new PC? Check copy scope, profile paths, and hidden items, then verify and recover safely."
seo_title: "Files Not Copied to New Computer: Fix Missing User Folders"
seo_description: "First copy finished but user folders are missing on the new PC? Check copy scope, profile paths, and hidden items, then verify and recover safely."
keywords:
  - "files not copied to new computer"
date: 2026-11-21T14:33:58+08:00
publishDate: 2026-11-21T14:33:58+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to the new Windows PC, but Desktop, Documents, or other files are absent.

## Check what the first copy actually included
Open File Explorer on the new PC, paste `%USERPROFILE%` into the address bar, and press Enter. Confirm whether Desktop, Documents, Downloads, Pictures, and Videos exist. If they are absent, the copy likely skipped them because the source paths differed or the job only covered a parent folder. Compare the source path on the old PC: right-click each user folder, choose Properties, and note the Location tab. If the source folder was redirected to another drive, the default user profile copy would not contain it.

## Check hidden and redirected locations
In File Explorer, enable View > Show > Hidden items. Look for folders such as OneDrive\Desktop or OneDrive\Documents. If files were stored in OneDrive, they may not appear under the local profile until sync completes. Also check the old PC's folder redirection settings; a redirected Documents folder may live on D:\Users or a network share, not under C:\Users.

## Verification test
Create a small test file on the old PC in Documents, copy it to the same relative path on the new PC, and confirm it appears. Then open the new PC's Documents folder and compare the item count with the source. If counts differ, the first copy was incomplete.

## Recovery note
Do not delete the source copy. Re-run the copy with the exact redirected paths included, or restore missing folders from your backup. If the source is intact, a targeted second copy is safe. For help mapping the correct paths,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).

If user folders remain absent after these checks, the **files not copied to new computer** issue is usually a path-scope problem, not data loss.
