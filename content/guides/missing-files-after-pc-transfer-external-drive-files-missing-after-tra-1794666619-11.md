---
title: "External Drive Files Missing After Transfer: Checking Hidden and Offloaded Data"
description: "A practical fix for external drive files missing after transfer on Windows. Check hidden files, offline attributes, and verify with a controlled test before recovery."
seo_title: "External Drive Files Missing After Transfer: Hidden Files and Offload Check"
seo_description: "A practical fix for external drive files missing after transfer on Windows. Check hidden files, offline attributes, and verify with a controlled test before recovery."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-24T12:00:19+08:00
publishDate: 2026-11-24T12:00:19+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

## Troubleshooting

You copied your user folders to an external drive, moved them to the new PC, and now the expected files are absent. Before assuming data loss, check whether Windows is hiding or offloading them. First, in File Explorer, open the external drive, go to View > Show > Hidden items. If your files appear, they were copied but marked hidden; right-click the folder, choose Properties, and clear Hidden. Next, right-click the drive, select Properties > Tools > Check, and let Windows scan for file system errors. If the scan reports no errors but files are still absent, check for offline attributes: open Command Prompt as administrator and run `attrib -O -P -S -H X:\*.* /S /D`, replacing X with your drive letter. This clears offline and pinned flags that can make files appear missing. A verification test: create a small test folder on the external drive, copy it to the new PC, and confirm it appears. Then repeat with one real user folder; if the test folder copies but the real folder does not, the original copy was incomplete. For rollback, do not write new data to the external drive; keep it connected and use the original PC as the source until you confirm the files. If these checks leave you stuck,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult) before running any recovery tool. This addresses the specific case of **external drive files missing after transfer**, where hidden or offline attributes mimic deletion.

Repeat the same check after a restart and confirm the result twice.

Repeat the same check after a restart and confirm the result twice.
