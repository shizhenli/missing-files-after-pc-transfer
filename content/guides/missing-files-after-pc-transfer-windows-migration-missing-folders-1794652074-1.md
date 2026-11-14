---
title: "Windows Migration Missing Folders: Restoring Desktop, Documents, and AppData"
description: "Desktop, Documents, or AppData folders missing after a Windows PC-to-PC migration? Follow these checks to diagnose the profile folder gap and restore the expected outcome."
seo_title: "Fix windows migration missing folders after PC transfer"
seo_description: "Desktop, Documents, or AppData folders missing after a Windows PC-to-PC migration? Follow these checks to diagnose the profile folder gap and restore the expected outcome."
keywords:
  - "windows migration missing folders"
date: 2026-11-14T19:18:45+08:00
publishDate: 2026-11-14T19:18:45+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

## Troubleshooting

You finished a Windows PC-to-PC migration, but your Desktop, Documents, or AppData folders are not where they should be. This points to a profile-folder copy gap, not a total data loss. Start by opening File Explorer and navigating to C:\Users. Look for your old profile folder name. If it exists but appears empty, right-click it, choose Properties, and check the size. A near-zero size means the folder structure copied but the contents did not. If the folder is absent entirely, the migration skipped the profile path. Next, check C:\Users\Public and any external drive used during transfer for a folder named Windows.old or a backup set. Open it and compare the folder names against your expected profile. If you find Desktop or Documents there, the data exists and only the final placement failed. A quick verification test: create a new text file on the old profile's Desktop path, then search the new PC for that filename using File Explorer search. If it appears under a different user path, the migration redirected rather than missed the files. Before making changes, note that moving folders back can overwrite newer files, so copy rather than cut, and keep the original backup until you confirm everything opens. This is a common **windows migration missing folders** case, and a controlled diagnosis usually restores the expected outcome. If the checks above leave the folders missing, stop copying and

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) so the profile path can be reviewed before further changes.
