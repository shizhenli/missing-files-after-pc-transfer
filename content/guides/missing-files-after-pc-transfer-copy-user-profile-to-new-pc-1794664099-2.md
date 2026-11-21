---
title: "Copy User Profile to New PC: When Desktop, Documents, and AppData Don't Appear"
description: "Desktop, Documents, or AppData folders missing after copying your user profile to a new PC? Follow these checks to diagnose and restore the expected folders."
seo_title: "Copy User Profile to New PC: Fix Missing Desktop, Documents, AppData"
seo_description: "Desktop, Documents, or AppData folders missing after copying your user profile to a new PC? Follow these checks to diagnose and restore the expected folders."
keywords:
  - "copy user profile to new pc"
date: 2026-11-21T14:30:50+08:00
publishDate: 2026-11-21T14:30:50+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user profile to a new PC, but Desktop, Documents, or AppData folders are missing—and you're stuck before any controlled diagnosis.

## Confirm the source profile path

On the old PC, open File Explorer and navigate to C:\Users. Verify the exact folder name (e.g., C:\Users\YourName). If the folder is missing or renamed, the copy used the wrong source. Result: an empty or partial destination.

## Check hidden items and AppData visibility

On the new PC, open File Explorer, go to View, and enable Hidden items. AppData is hidden by default. If you see AppData now, the copy succeeded but was hidden. If Desktop or Documents are still absent, the copy skipped them.

## Inspect the copy method

If you used a manual drag-and-drop, Windows may have merged folders incorrectly. Check whether the destination contains nested folders like C:\Users\YourName\Desktop\Desktop. That indicates a path error, not data loss.

## Verification test

Create a test file on the old PC's Desktop named test-profile.txt. Copy the profile again using a tool that preserves folder structure, such as robocopy with /E. After copying, confirm test-profile.txt appears in C:\Users\YourName\Desktop on the new PC. If it does, the profile copied correctly.

## Rollback and recovery

Before retrying, rename the incomplete destination folder (e.g., YourName_old) instead of deleting it. This preserves any partial data. Then perform a fresh **copy user profile to new pc** using a method that includes hidden and system folders.

If folders remain missing after these checks, stop and

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before making further changes.
