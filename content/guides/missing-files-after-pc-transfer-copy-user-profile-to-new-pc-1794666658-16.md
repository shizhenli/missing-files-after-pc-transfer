---
title: "Copy User Profile to New PC: Missing Desktop, Documents, and AppData After Migration"
description: "After copying your user profile to a new PC, Desktop, Documents, or AppData folders are missing. Follow these checks to diagnose and restore your profile folders."
seo_title: "Copy User Profile to New PC: Fix Missing Desktop, Documents, and AppData"
seo_description: "After copying your user profile to a new PC, Desktop, Documents, or AppData folders are missing. Follow these checks to diagnose and restore your profile folders."
keywords:
  - "copy user profile to new pc"
date: 2026-11-25T12:00:09+08:00
publishDate: 2026-11-25T12:00:09+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user profile to a new PC, but now Desktop, Documents, or AppData folders are missing. This usually means the copy skipped hidden or locked profile folders, or the new PC created a fresh profile instead of using the transferred one.

## Check the source and destination paths

On the old PC, open File Explorer and navigate to C:\Users. Confirm your profile folder name (e.g., C:\Users\YourName). Then on the new PC, go to C:\Users and compare. If the new PC shows a different folder name, Windows created a new profile and your files may be in the old one. Also check that you copied the entire profile folder, not just visible subfolders. Hidden folders like AppData are often missed because File Explorer hides them by default. Enable hidden items via View > Show > Hidden items.

## Verify folder contents and permissions

Open the copied profile folder on the new PC. If Desktop, Documents, or AppData are absent, the copy likely failed due to access denied errors. Right-click the folder, choose Properties > Security, and confirm your new account has Read & Execute permissions. If not, take ownership or copy again using an administrator account.

## Run a verification test

Create a test file on the old PC's Desktop, then copy the profile again using a tool that preserves hidden files (e.g., robocopy with /E /COPYALL). After copying, check if the test file appears on the new PC's Desktop. If it does, the copy method works; if not, the issue is permissions or profile redirection.

## Rollback and recovery

Before making changes, back up the new PC's current profile folder. If the copy overwrote something important, restore from that backup. To avoid data loss, always keep the old PC unchanged until you confirm the new profile works.

If these steps don't restore your folders,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) for a guided diagnosis. For a reliable **copy user profile to new pc**, ensure hidden files are included and permissions are correct.
