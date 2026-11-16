---
title: "Copy User Profile to New PC: When Desktop, Documents, and AppData Are Missing"
description: "Fix a Windows profile copy that misses Desktop, Documents, or AppData folders. Check source paths, hidden items, and permissions, then verify with a test file."
seo_title: "Copy User Profile to New PC: Fix Missing Desktop, Documents & AppData"
seo_description: "Fix a Windows profile copy that misses Desktop, Documents, or AppData folders. Check source paths, hidden items, and permissions, then verify with a test file."
keywords:
  - "copy user profile to new pc"
date: 2026-11-16T09:00:06+08:00
publishDate: 2026-11-16T09:00:06+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

## Check the source profile path first

You copied your user profile to a new PC, but Desktop, Documents, or AppData folders are absent, and you are stuck before any controlled diagnosis. Start by confirming the exact source path. On the old PC, open File Explorer and navigate to C:\Users. Locate your profile folder and note its exact name. If the folder is named Default or Public, you are looking at the wrong profile. The correct folder usually matches your Windows username and contains Desktop, Documents, and AppData. If those subfolders are missing there, the source is incomplete and no copy method will recover them.

## Verify hidden items and permissions

Next, enable hidden items in File Explorer on both PCs. AppData is hidden by default, so it may exist but be invisible. Then check permissions: right-click the source profile folder, choose Properties, Security, and confirm your account has Read access. If access is denied, take ownership or copy from an administrator account. When copying, use a method that preserves folder structure, such as robocopy with /E, rather than dragging only visible files.

## Run a verification test

Create a test file on the old PC Desktop, then repeat the **copy user profile to new pc** step. After the transfer, open C:\Users\<YourName> on the new PC and confirm the test file appears alongside Desktop, Documents, and AppData. If it does not, the copy is still incomplete. If it does, the structure is correct and you can proceed with the remaining data.

## Rollback and recovery note

Before retrying, rename the incomplete profile folder on the new PC to something like Profile_Old. This preserves any partial data and lets Windows rebuild a clean profile if needed. If the source folders remain missing after these checks, stop and

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before making further changes.
