---
title: "Windows Migration Missing Folders: Diagnosing an Incomplete User Profile Copy"
description: "Desktop, Documents, or AppData folders missing after a Windows PC-to-PC migration? Diagnose an incomplete user profile copy and restore the expected folders."
seo_title: "Windows Migration Missing Folders: Fix an Incomplete User Profile Copy"
seo_description: "Desktop, Documents, or AppData folders missing after a Windows PC-to-PC migration? Diagnose an incomplete user profile copy and restore the expected folders."
keywords:
  - "windows migration missing folders"
date: 2026-11-24T11:00:08+08:00
publishDate: 2026-11-24T11:00:08+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

**windows migration missing folders**. You finished a Windows PC-to-PC migration, opened the new machine, and found Desktop, Documents, or AppData folders absent from the user profile.

## Confirm what actually transferred

Open File Explorer on the new PC and go to C:\Users\<your-username>. Compare the folder list against the old PC's C:\Users\<your-username>. If Desktop, Documents, or AppData are missing entirely, the copy stopped before the profile finished. If the folders exist but are empty, the copy created the folder shell without contents. Note which case you see, because they point to different causes.

Next, check whether the folders were redirected. Right-click Desktop or Documents, choose Properties, and read the Location tab. A path pointing to OneDrive or another drive means the data may exist elsewhere, not that it was lost.

## Check the source and the copy method

On the old PC, confirm the folders still exist under C:\Users\<your-username>. If they do, the source is intact and the transfer itself was incomplete. Review how you copied: a manual drag-and-drop of the profile folder often skips hidden items such as AppData. Enable Show hidden items in File Explorer's View options and recheck the destination.

## Verification test

Create a small test file on the old PC's Desktop, copy the Desktop folder again to the new profile, and confirm the file appears. If it does, the method works and you can repeat it for Documents and AppData. If it does not, stop and diagnose permissions before copying more.

## Rollback note

Do not delete anything on the old PC until the new profile is verified. Keep the old drive untouched as your recovery source.

If these checks leave the folders missing,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before making further changes.
