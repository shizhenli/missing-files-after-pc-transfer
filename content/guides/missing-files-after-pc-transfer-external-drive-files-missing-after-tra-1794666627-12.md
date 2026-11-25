---
title: "External Drive Copy Incomplete: Why Fewer Files Appear After Transfer"
description: "External drive shows fewer files than the source after a PC-to-PC transfer? Diagnose the incomplete copy with size, count, and hidden-file checks, then restore safely."
seo_title: "External Drive Files Missing After Transfer: Fix an Incomplete Copy"
seo_description: "External drive shows fewer files than the source after a PC-to-PC transfer? Diagnose the incomplete copy with size, count, and hidden-file checks, then restore safely."
keywords:
  - "external drive files missing after transfer"
date: 2026-11-25T08:00:11+08:00
publishDate: 2026-11-25T08:00:11+08:00
draft: false
categories:
  - "File Migration"
category_slug: "file-migration"
---

You copied your user folders to an external drive during a PC-to-PC migration, but the drive now shows fewer files than the source. That points to an incomplete copy, not necessarily lost data. Let's confirm what actually made it across before you change anything.

## Check the copy at the folder level
Open the source user folder and the matching folder on the external drive side by side. Right-click each folder, choose Properties, and compare the total size and file count. A large gap in size means files never copied; a matching size with a lower count usually means hidden items are simply not displayed. In File Explorer, enable View > Show > Hidden items and compare again.

## Confirm whether the copy stopped early
Look for files with temporary extensions such as .tmp or .crdownload, and check whether the last-modified timestamps stop at a single point. If they do, the transfer was interrupted, which explains why **external drive files missing after transfer** appear as a partial set rather than random losses.

## Run a verification test
Create a small test folder in the source with three files, copy it to the external drive, and confirm all three arrive. Then copy one large folder again and watch for an error dialog or a silent stop. If the test folder copies fully but the large folder does not, the problem is transfer stability or free space, not the source data.

## Recovery and rollback note
Do not delete the source folders until the copy is verified. Re-run the copy with a tool that logs errors, and keep the original drive untouched as your rollback point. If the source itself is now incomplete, stop writing to both drives and seek recovery advice before proceeding.

If these checks leave you unsure,

![A file comparison list on a laptop during a Windows migration](/images/service-detail-960.webp "Windows file migration comparison")

[Ask for help](/#consult).
