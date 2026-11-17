---
title: "Windows Migration Missing Folders: What to Check Before You Re-Copy"
description: "Desktop, Documents, or AppData folders missing after a PC-to-PC migration? Follow these checks to diagnose the incomplete copy and restore your user profile folders."
seo_title: "Windows Migration Missing Folders: Fix Desktop, Documents, AppData"
seo_description: "Desktop, Documents, or AppData folders missing after a PC-to-PC migration? Follow these checks to diagnose the incomplete copy and restore your user profile folders."
keywords:
  - "windows migration missing folders"
date: 2026-11-17T09:01:41+08:00
publishDate: 2026-11-17T09:01:41+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You finished a Windows PC-to-PC migration, but Desktop, Documents, or AppData folders are missing from the new profile. Before you copy anything again, confirm what actually transferred. This is a common case of **windows migration missing folders**, and a controlled diagnosis prevents overwriting good data.

## Check the source profile path first

On the old PC, open File Explorer and paste `C:\Users` into the address bar. Confirm your old account folder exists and contains Desktop, Documents, and AppData. If AppData is hidden, enable Show hidden items in View. Result interpretation: if the folders exist on the source but not on the destination, the transfer skipped them rather than the data being gone.

## Check the destination profile and copy method

On the new PC, open `C:\Users\<YourName>`. Compare the folder list with the source. Then review how you migrated: a manual drag-and-drop or a tool set to skip hidden or system items will omit AppData. Result interpretation: a missing AppData on the destination while present on the source points to a hidden-folder exclusion, not corruption.

## Verification test

Create a small test file on the old PC's Desktop, copy the Desktop folder to the new profile, and confirm the file appears. If it does, the path and permissions are sound and only the original copy was incomplete.

## Rollback and recovery note

Do not delete the old drive or profile until the new one is verified. If a partial copy already merged folders, restore the previous state from a backup or File History before retrying, so you can compare cleanly.

If the source folders are also absent, stop and get a second opinion:

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
