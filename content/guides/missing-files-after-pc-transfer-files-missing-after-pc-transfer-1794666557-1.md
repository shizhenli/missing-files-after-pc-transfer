---
title: "User Folders Empty After PC Transfer? Check the Copy Scope First"
description: "First copy finished but user folders are empty on the new PC? Diagnose copy scope, hidden profiles, and redirects before re-copying, with a safe rollback note."
seo_title: "Files Missing After PC Transfer: Fix the Empty User Folder Copy"
seo_description: "First copy finished but user folders are empty on the new PC? Diagnose copy scope, hidden profiles, and redirects before re-copying, with a safe rollback note."
keywords:
  - "files missing after pc transfer"
date: 2026-11-23T09:00:05+08:00
publishDate: 2026-11-23T09:00:05+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to the new PC, the progress bar finished, but Desktop, Documents, and Pictures are empty on the new machine. This is the classic **files missing after pc transfer** symptom, and it usually means the copy captured the wrong scope, not that the files vanished. Before re-copying anything, run these checks.

## Check 1: Confirm the source folder actually contains files

On the old PC, open File Explorer, paste `%USERPROFILE%` in the address bar, and press Enter. Open Desktop, Documents, and Pictures. If they show files here, the source is fine. If they are empty here too, the data lives elsewhere (OneDrive or a redirected folder) and the copy had nothing to grab.

## Check 2: Look for a second profile folder on the new PC

On the new PC, open `C:\Users`. You may see two folders: your new account and a second one named like `OldName` or `OldName.PCNAME`. Open the second one. If your files are inside it, the copy landed in a separate profile, not your active one. Result interpretation: files present in the second folder means the transfer worked but targeted the wrong profile.

## Check 3: Verify folder redirection and OneDrive

Right-click Desktop, choose Properties, and open the Location tab. If the path points to OneDrive, your files are in the cloud folder, not the local profile. Repeat for Documents and Pictures. A copy of the local profile will then look empty.

## Verification test

Create a test file on the old PC Desktop, copy it manually to the new PC Desktop, and confirm it appears. If it does, the destination is writable and the earlier copy simply missed the source path.

## Rollback and recovery note

Do not delete the old PC profile or the second folder on the new PC until the verification test passes. Keep the original drive untouched as your rollback source.

If these checks do not explain the gap,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) with your folder paths and we will review the copy scope.
