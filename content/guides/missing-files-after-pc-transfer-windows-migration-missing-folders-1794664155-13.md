---
title: "Windows Migration Missing Folders: Diagnosing a Profile Folder That Didn't Arrive"
description: "Desktop, Documents, or AppData folders missing after a Windows PC-to-PC migration? Follow these checks to confirm what was skipped and restore the expected profile folders."
seo_title: "Windows Migration Missing Folders: Fix Desktop, Documents, AppData"
seo_description: "Desktop, Documents, or AppData folders missing after a Windows PC-to-PC migration? Follow these checks to confirm what was skipped and restore the expected profile folders."
keywords:
  - "windows migration missing folders"
date: 2026-11-21T14:37:04+08:00
publishDate: 2026-11-21T14:37:04+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You finished a Windows PC-to-PC migration, but when you open the new profile, Desktop, Documents, or AppData is simply not there. Before you copy anything again, confirm what the migration actually did, because **windows migration missing folders** usually means the profile was only partially transferred.

## Check the source profile path first

On the old PC, open File Explorer and paste `C:\Users` into the address bar. You should see your old account folder. Open it and look for Desktop, Documents, and AppData. If AppData is hidden, enable hidden items in View. If the folders exist on the source but not on the destination, the migration skipped user-profile content rather than losing it.

## Compare the destination profile

On the new PC, open `C:\Users\<YourName>`. If the folder exists but is nearly empty, the transfer created the profile shell without the contents. If the folder is missing entirely, the migration never created the profile. Either result means you can recover from the source; do not run another full migration until you know which case you have.

## Verification test

Create a small test file on the old PC's Desktop, then copy that single file manually to the new Desktop. If it appears, the destination profile is writable and the original migration simply omitted folders. If it does not appear, stop and check permissions on the destination profile before copying more.

## Recovery note

Keep the old drive unchanged until recovery is complete. Copy Desktop, Documents, and AppData from the source profile into the matching destination folders, then sign out and back in. If AppData will not copy due to locks, copy it from an offline source or a backup. For a guided diagnosis,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
