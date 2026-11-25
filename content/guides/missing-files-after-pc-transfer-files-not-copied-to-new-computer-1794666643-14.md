---
title: "Why Your First Copy Skips User Folders and How to Recover Them"
description: "First copy finished but user folders are missing on the new PC? Check hidden items, copy logs, and folder redirection, then verify and recover safely."
seo_title: "Files Not Copied to New Computer: Fix Missing User Folders"
seo_description: "First copy finished but user folders are missing on the new PC? Check hidden items, copy logs, and folder redirection, then verify and recover safely."
keywords:
  - "files not copied to new computer"
date: 2026-11-25T10:00:05+08:00
publishDate: 2026-11-25T10:00:05+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You finished the first copy, but when you open File Explorer on the new PC, the user folders you expected are simply not there. This is a common case of **files not copied to new computer** during a Windows PC-to-PC migration, and it usually points to a copy that skipped hidden or redirected content rather than a failed drive.

## Check What the Copy Actually Included

Open the source PC and enable hidden items in File Explorer (View > Show > Hidden items). Then compare the top-level user folder (C:\Users\YourName) on both PCs. If Desktop, Documents, or AppData are missing on the new PC but visible on the source, the copy tool skipped hidden or system-protected items. Also check whether those folders are redirected to OneDrive: right-click Documents > Properties > Location. If the path points to a OneDrive folder, the local user folder may be nearly empty by design.

## Interpret the Result

If the source folders are empty too, the data was never in the default location, so look for the real path before copying again. If the source has files but the destination does not, the first copy was incomplete. Do not run a second full copy over the top yet.

## Verification Test

Create a small test folder on the source Desktop with one text file, copy it manually to the same location on the new PC, and confirm it appears. This proves the destination path is writable and not redirected.

## Rollback and Recovery

Before retrying, rename the incomplete destination user folder (for example, YourName_old) so nothing is overwritten. Then copy again with a tool that preserves hidden files, and keep the renamed folder until you confirm everything is present. If the source data is unclear,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before deleting anything.
