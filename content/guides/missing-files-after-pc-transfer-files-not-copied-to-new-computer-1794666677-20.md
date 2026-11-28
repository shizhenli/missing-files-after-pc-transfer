---
title: "Files Not Copied to New Computer: Why the First Copy Misses User Folders"
description: "First copy finished but user folders are missing on the new PC? Learn how to check copy scope, verify hidden folders, and recover without losing data."
seo_title: "Files Not Copied to New Computer: Fix Missing User Folders"
seo_description: "First copy finished but user folders are missing on the new PC? Learn how to check copy scope, verify hidden folders, and recover without losing data."
keywords:
  - "files not copied to new computer"
date: 2026-11-28T21:40:59+08:00
publishDate: 2026-11-28T21:40:59+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

## Troubleshooting

You finished the first copy to your new Windows PC, but your Desktop, Documents, or Downloads folders are simply not there. Before you recopy everything, check whether the job copied the folder contents rather than the user profile itself. In File Explorer, open the destination drive and look for a folder named after your old username. If it exists but is empty, the copy likely selected only top-level folders and skipped subfolders. If it does not exist, the source path may have pointed to a shortcut or a redirected OneDrive folder, so the actual files were never in scope. Next, enable hidden items in File Explorer and confirm whether AppData and other hidden user folders are present; their absence usually means the copy tool ignored hidden system files. Also compare the total size of the source user folder with the destination folder. A large mismatch confirms an incomplete copy, while a close match suggests a display or permissions issue. As a verification test, create a small text file on the old PC desktop, copy it manually to the new PC desktop, and confirm it appears. If it does, the original copy missed files rather than the destination being unwritable. Before retrying, keep the old PC unchanged as your rollback source, and do not delete anything from it until the new PC passes the same test. If these checks show **files not copied to new computer** because of profile redirection or hidden folders, stop repeating the same copy and

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) to map the correct source paths safely.
