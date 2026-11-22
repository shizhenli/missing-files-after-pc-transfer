---
title: "Windows Migration Missing Folders: When Desktop, Documents, or AppData Don't Appear"
description: "Desktop, Documents, or AppData folders missing after a Windows PC-to-PC migration? Follow these checks to diagnose and restore your user profile folders."
seo_title: "Windows Migration Missing Folders: Fix Missing User Profile Folders"
seo_description: "Desktop, Documents, or AppData folders missing after a Windows PC-to-PC migration? Follow these checks to diagnose and restore your user profile folders."
keywords:
  - "windows migration missing folders"
date: 2026-11-22T11:00:09+08:00
publishDate: 2026-11-22T11:00:09+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You finished migrating to a new PC, but Desktop, Documents, or AppData folders are missing from your user profile.

## Confirm What Actually Copied

Open File Explorer and navigate to C:\Users\<your-username>. Compare the folder list against your old PC. If Desktop, Documents, or AppData are absent, the migration tool skipped them—often because they were redirected to OneDrive or another drive. Check the old PC's folder properties: right-click Documents, choose Properties, and look at the Location tab. If it points to a OneDrive path, the files exist but under a different folder. Also check C:\Users\Default for stray profile data.

## Check Hidden and System Folders

AppData is hidden by default. In File Explorer, enable View > Show > Hidden items. If AppData still doesn't appear, it wasn't copied. This is a common cause of **windows migration missing folders** during profile transfers.

## Run a Verification Test

Create a test file on the old PC's Desktop, then check whether it appears on the new PC after a manual copy. If it does, the migration tool—not Windows—caused the gap. If it doesn't, permissions or OneDrive sync may be blocking access.

## Recovery and Rollback

Before making changes, keep the old PC untouched. Manually copy the missing folders from C:\Users\<old-username> to the new profile using an external drive. If AppData is involved, copy it while logged into a different admin account to avoid file locks. Do not delete the old profile until you confirm everything opens correctly.

If these steps don't restore the folders,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) with your migration tool name and folder paths.
