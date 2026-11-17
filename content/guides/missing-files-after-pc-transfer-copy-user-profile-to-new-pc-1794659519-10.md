---
title: "Copy User Profile to New PC: Restoring Missing Desktop, Documents, and AppData Folders"
description: "Fix missing user profile folders after PC migration. Learn to verify, restore Desktop, Documents, and AppData folders when the copy user profile to new PC step fails."
seo_title: "Copy User Profile to New PC: Fix Missing Desktop, Documents, AppData"
seo_description: "Fix missing user profile folders after PC migration. Learn to verify, restore Desktop, Documents, and AppData folders when the copy user profile to new PC step fails."
keywords:
  - "copy user profile to new pc"
date: 2026-11-17T10:00:07+08:00
publishDate: 2026-11-17T10:00:07+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your profile to a new PC, but Desktop, Documents, or AppData folders are missing—this happens when the migration skips user profile folders before diagnosis. Here’s how to restore them.

## Check the Source Profile Path
On the old PC, open File Explorer and navigate to C:\Users. Confirm the exact folder name for your profile (e.g., C:\Users\YourName). If it’s not there, check C:\Users\Public or a backup drive. Result interpretation: if the source folder exists but is empty, the copy likely failed silently; if it’s missing entirely, the profile was never created or was moved.

## Verify the Destination Folder Structure
On the new PC, go to C:\Users. You should see a folder matching your old profile name. If it’s absent, the migration didn’t create it. If present but missing subfolders like Desktop, Documents, or AppData, the copy was incomplete. Manually create the missing subfolders only after confirming the source has them—otherwise, you’ll copy emptiness.

## Perform a Controlled Copy Test
Open Command Prompt as administrator. Run: robocopy "C:\Users\OldName" "C:\Users\NewName" /E /COPYALL /R:1 /W:1 /LOG:C:\copy.log. This copies all subdirectories and permissions. After it finishes, open C:\copy.log and search for “ERROR” or “FAILED.” If errors appear, note the file paths—they often point to locked AppData files. Close all apps and retry. This is the reliable way to **copy user profile to new pc** without missing folders.

## Verification Test
Open the new profile’s Desktop, Documents, and AppData folders. Compare file counts with the source using right-click > Properties. If counts match, the copy succeeded. If not, check the log for skipped items.

## Rollback and Recovery
If the copy overwrote existing files, restore from a backup or use File History. Before retrying, rename the destination profile folder to avoid conflicts. For persistent issues,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) to diagnose the migration step.
