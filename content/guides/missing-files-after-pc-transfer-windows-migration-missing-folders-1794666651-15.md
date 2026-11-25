---
title: "Windows Migration Missing Folders: Fixing an Incomplete User Profile Copy"
description: "Fix windows migration missing folders by checking copy scope, hidden folders, and profile paths. Step-by-step diagnosis for Desktop, Documents, and AppData."
seo_title: "Windows Migration Missing Folders: Restore User Profile Folders"
seo_description: "Fix windows migration missing folders by checking copy scope, hidden folders, and profile paths. Step-by-step diagnosis for Desktop, Documents, and AppData."
keywords:
  - "windows migration missing folders"
date: 2026-11-25T11:00:08+08:00
publishDate: 2026-11-25T11:00:08+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You migrated to a new PC and now Desktop, Documents, or AppData folders are missing from your user profile. This usually means the transfer tool skipped hidden or system-protected folders rather than losing data.

## Check the Copy Scope and Hidden Items

First, on the new PC, open File Explorer and navigate to C:\Users\<your-username>. Enable hidden items via View > Show > Hidden items. If you see Desktop, Documents, or AppData now, the files were copied but hidden. If they are still absent, the migration tool likely excluded them. Check the tool's log or summary for skipped items. A common cause is that the tool copied only visible folders and ignored AppData because it is hidden by default.

## Verify the Source Profile Path

On the old PC, confirm the actual folder locations. Open File Explorer, right-click Desktop or Documents, and choose Properties > Location. If the path points to OneDrive or another drive, the migration may have looked in the wrong place. Copy those folders manually to the new profile, then compare file counts.

## Run a Verification Test

Create a test file on the old PC's Desktop and Documents. Copy both folders manually to the new PC's corresponding user folder. If the test files appear, the original migration missed them due to scope or path issues. This confirms the fix: recopy the missing folders with hidden items enabled.

## Rollback and Recovery Note

Before recopying, do not delete anything on the new PC. If the manual copy overwrites existing files, restore from the old PC or a backup. Keep the old profile intact until you verify all folders are present.

If these checks do not restore the folders, the migration may have used a profile that excluded system folders. For a controlled diagnosis of **windows migration missing folders**,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
