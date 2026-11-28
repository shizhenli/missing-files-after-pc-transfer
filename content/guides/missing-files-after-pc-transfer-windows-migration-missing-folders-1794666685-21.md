---
title: "Migration Misses User Profile Folders: A Controlled Diagnosis"
description: "Fix Windows migration missing folders by checking profile paths, hidden AppData, and copy scope. Step-by-step diagnosis to restore Desktop, Documents, and AppData after PC transfer."
seo_title: "Windows Migration Missing Folders: Diagnose Missing Desktop, Documents, AppData"
seo_description: "Fix Windows migration missing folders by checking profile paths, hidden AppData, and copy scope. Step-by-step diagnosis to restore Desktop, Documents, and AppData after PC transfer."
keywords:
  - "windows migration missing folders"
date: 2026-11-28T21:40:59+08:00
publishDate: 2026-11-28T21:40:59+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You migrated to a new PC and now Desktop, Documents, or AppData folders are missing from your user profile. This points to a copy-scope or profile-path issue, not data loss. Here is how to diagnose it.

## Check the actual profile path
Open File Explorer and paste `%USERPROFILE%` into the address bar. Press Enter. You should land in `C:\Users\<YourName>`. If you land in a different folder name, the migration created a new profile instead of copying the old one. Result: the old folders exist under the previous profile name and were never merged. Check `C:\Users` for a second folder matching your old username.

## Check hidden AppData
AppData is hidden by default. In File Explorer, enable View > Hidden items. Then open `%USERPROFILE%\AppData`. If AppData is absent entirely, the migration tool skipped hidden folders. If it exists but is nearly empty, the copy stopped before hidden content was transferred.

## Check copy scope
Compare the source and destination folder counts. On the old PC, open `C:\Users\<YourName>` and note the folders present. On the new PC, open the same path. Missing Desktop, Documents, or AppData means the tool copied only visible top-level items. This is the common cause of **windows migration missing folders**.

## Verification test
Create a test file on the old PC Desktop, then run the same migration step again. If the test file does not appear on the new PC, the copy scope is still wrong and must be corrected before retrying.

## Rollback and recovery
Do not delete the old profile or source drive until verification passes. If folders are still missing, copy them manually from the old profile to the matching new profile path, then confirm each folder opens.

If the profile path or copy scope remains unclear,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
