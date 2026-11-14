---
title: "Copy User Profile to New PC: Fixing Missing Desktop, Documents, and AppData Folders"
description: "Fix missing Desktop, Documents, or AppData folders after copying a user profile to a new PC. Step-by-step diagnosis and recovery."
seo_title: "Copy User Profile to New PC: Fix Missing User Folders"
seo_description: "Fix missing Desktop, Documents, or AppData folders after copying a user profile to a new PC. Step-by-step diagnosis and recovery."
keywords:
  - "copy user profile to new pc"
date: 2026-11-14T19:18:45+08:00
publishDate: 2026-11-14T19:18:45+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user profile to a new PC, but now Desktop, Documents, or AppData folders are missing. This usually means the copy skipped hidden or system-protected folders, or the profile path was wrong.

## Check the Source and Destination Paths

First, confirm where the old profile actually lived. On the old PC, open File Explorer and go to C:\Users. You should see your username folder. If you copied from a different path, like a backup drive, verify that the backup contains the missing folders. On the new PC, check C:\Users\YourUsername. If the folders are not there, the copy missed them.

## Check for Hidden Folders and Permissions

AppData is hidden by default. In File Explorer, enable View > Hidden items. Then navigate to C:\Users\YourUsername. If AppData appears, the copy may have skipped it because it was hidden. Also, right-click the folder and check Properties > Security. If your new account lacks permissions, the copy may have failed silently.

## Verify with a Test Copy

Create a test folder on the new PC, then copy one missing folder manually from the source. For example, copy Desktop from the old profile to the new one. If it copies without error, the original transfer method was the problem. If it fails, note the error message.

## Rollback and Recovery

Before retrying, do not overwrite the new profile. Instead, rename the incomplete profile folder to YourUsername_old, then create a fresh profile. Use a reliable method to **copy user profile to new pc** again, ensuring hidden items are included. If you are unsure,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before making changes.

## Final Verification

After copying, open each folder and confirm files are present. Check AppData\Roaming for application settings. If all folders appear and open correctly, the migration is complete.
