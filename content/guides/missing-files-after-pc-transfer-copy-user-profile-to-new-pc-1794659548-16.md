---
title: "Copy User Profile to New PC: Fixing Missing Desktop, Documents, and AppData After Migration"
description: "Missing user profile folders after copying to a new PC? Learn how to diagnose and fix missing Desktop, Documents, and AppData folders with a controlled check."
seo_title: "Copy User Profile to New PC: Fix Missing Desktop, Documents, AppData"
seo_description: "Missing user profile folders after copying to a new PC? Learn how to diagnose and fix missing Desktop, Documents, and AppData folders with a controlled check."
keywords:
  - "copy user profile to new pc"
date: 2026-11-18T10:01:33+08:00
publishDate: 2026-11-18T10:01:33+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user profile to a new PC, but now the Desktop, Documents, or AppData folders are missing—this guide helps you diagnose and fix that specific failure.

## Check the source profile path

First, confirm the original profile folder was fully accessible. On the old PC, open File Explorer and navigate to C:\Users\[YourUsername]. Verify that Desktop, Documents, and AppData are visible. If AppData is hidden, enable "Hidden items" in the View tab. If any folder is missing here, the copy never had the data—recover it from a backup or restore point before proceeding.

## Verify the copy destination

On the new PC, check C:\Users\[YourUsername]. Compare the folder list with the source. If Desktop or Documents are absent, the copy likely skipped them due to permission errors or an interrupted transfer. Look for a folder named "Desktop" inside another location, such as C:\Users\Public or a temp folder. If AppData is missing, note that it is hidden by default—enable hidden items again. If the folders are truly absent, the copy was incomplete.

## Run a verification test

Create a test file on the old PC's Desktop (e.g., test.txt). Copy the entire user profile folder again using a tool that preserves permissions, such as Robocopy with /COPYALL. After the copy, check if test.txt appears on the new PC's Desktop. If it does, the profile copied correctly. If not, the issue is with the copy method or permissions.

## Rollback and recovery

Before retrying, create a restore point on the new PC. If the copy fails again, roll back to that point to avoid a half-migrated profile. For a clean slate, you can also use Windows' built-in "**Copy user profile to new pc**" feature via Settings > Accounts > Sync your settings, but ensure you have a backup first.

If these steps don't resolve the missing folders,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) for a guided diagnosis.
