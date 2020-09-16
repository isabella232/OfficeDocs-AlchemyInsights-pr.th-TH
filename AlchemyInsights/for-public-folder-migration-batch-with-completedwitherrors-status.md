---
title: สำหรับชุดการโยกย้ายโฟลเดอร์สาธารณะที่มีสถานะ CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744132"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>สำหรับชุดการโยกย้ายโฟลเดอร์สาธารณะที่มีสถานะ CompletedWithErrors

ใช้ขั้นตอนต่อไปนี้เพื่อทำให้ชุดงานเสร็จสมบูรณ์การข้ามรายการขนาดใหญ่/ไม่ถูกต้อง: 
1. อนุมัติรายการที่ถูกข้ามในชุดการโอนย้าย:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. ใช้คำสั่งต่อไปนี้เพื่ออนุมัติรายการที่ถูกข้ามในการร้องขอการโยกย้ายที่ "ซิงค์" แต่ยังไม่เสร็จสมบูรณ์:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. ชุดการโยกย้ายและการร้องขอควรดำเนินการต่อและดำเนินการต่อในเวลาไม่กี่นาที

