---
title: "Files Not Copied to New Computer: Why User Folders Are Missing After the First Copy"
description: "First copy finished but your user folders are missing on the new PC? Follow these checks to diagnose why files not copied to new computer and restore them."
seo_title: "Files Not Copied to New Computer: Fix Missing User Folders"
seo_description: "First copy finished but your user folders are missing on the new PC? Follow these checks to diagnose why files not copied to new computer and restore them."
keywords:
  - "files not copied to new computer"
date: 2026-11-18T09:00:06+08:00
publishDate: 2026-11-18T09:00:06+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You finished the first copy from your old Windows PC to the new one, but when you open File Explorer, your Desktop, Documents, and other user folders are simply not there. This is a common stop point in a PC-to-PC migration, and it usually means the copy targeted the wrong folder or skipped hidden profile data. Let's check a few things before you recopy anything.

## Check the copy destination path

On the new PC, open File Explorer and navigate to C:\Users. You should see a folder named after your old account. If it exists but is empty, the copy may have landed in Public or in a differently named profile. Right-click the folder, choose Properties, and compare the size to the source. A near-zero size confirms the copy did not include your user data.

## Check hidden items and permissions

In File Explorer, enable View > Show > Hidden items. Many user folders such as AppData are hidden by default, so they may be present but invisible. Also right-click the destination folder and check Security permissions; if your new account lacks read access, files can appear absent.

## Run a verification test

Create a small test file on the old PC's Desktop, then copy it manually to C:\Users\[YourName]\Desktop on the new PC. If it appears, the path is correct and the earlier copy was incomplete. If it does not, the destination profile is wrong.

## Rollback and recovery note

Do not delete the source copy. If the destination is wrong, remove only the empty or partial folder you created on the new PC, then recopy to the correct path. If **files not copied to new computer** remains unresolved after these checks,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before making further changes.
