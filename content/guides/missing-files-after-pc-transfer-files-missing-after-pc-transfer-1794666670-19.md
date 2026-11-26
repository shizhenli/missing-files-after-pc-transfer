---
title: "Files Missing After PC Transfer: Verifying the Copy Before You Re-Copy"
description: "First copy finished but user folders are empty on the new PC? Learn how to verify the copy, interpret results, and recover without overwriting."
seo_title: "Files Missing After PC Transfer: Verify the Copy First"
seo_description: "First copy finished but user folders are empty on the new PC? Learn how to verify the copy, interpret results, and recover without overwriting."
keywords:
  - "files missing after pc transfer"
date: 2026-11-26T09:59:16+08:00
publishDate: 2026-11-26T09:59:16+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You finished the first copy from your old Windows PC to the new one, but when you open File Explorer the user folders are empty and your documents are nowhere to be found.

## Check the source before touching the destination

On the old PC, open File Explorer and navigate to C:\Users\<your-username>. Right-click each expected folder (Desktop, Documents, Downloads, Pictures) and choose Properties. Read the Size and Contains values. If Size shows 0 bytes or Contains shows 0 Files, the source folder is empty and the copy had nothing to move. If Size is non-zero, the data exists and the problem is on the destination side.

## Check the destination path and hidden items

On the new PC, open C:\Users\<your-username> and enable View > Show > Hidden items. Confirm whether the folders exist but appear empty. Then right-click the same folders and compare Size and Contains against the source. A destination folder with 0 bytes while the source is non-zero confirms an incomplete copy. A destination folder that is missing entirely points to a path mismatch, often because the new PC created a different username.

## Verification test

Create a small test file on the old PC inside Documents, copy it manually to the new PC's Documents folder, and confirm it appears. If the test file arrives but the bulk copy did not, the original transfer stopped early rather than failing silently.

## Rollback and recovery note

Do not delete anything on the old PC or overwrite the new profile until you have confirmed the source sizes. Keep the old drive untouched as your recovery copy, then re-run the copy into the correct user path. If the source sizes are zero, stop and investigate the original profile before repeating the transfer.

If these checks leave you unsure which side is incomplete,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before making further changes to either PC.

A controlled diagnosis of why **files missing after pc transfer** occurs prevents a second copy from repeating the same gap.
