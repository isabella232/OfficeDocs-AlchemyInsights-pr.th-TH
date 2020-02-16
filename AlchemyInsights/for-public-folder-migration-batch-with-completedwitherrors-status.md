---
title: สำหรับชุดงานการโยกย้ายโฟลเดอร์สาธารณะที่มีสถานะ CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043625"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>สำหรับชุดงานการโยกย้ายโฟลเดอร์สาธารณะที่มีสถานะ CompletedWithErrors

ใช้ขั้นตอนต่อไปนี้เพื่อทำให้ชุดงานการข้ามรายการขนาดใหญ่/ไม่ถูกต้อง: 
1. อนุมัติรายการที่ถูกข้ามในแบทช์การย้าย:

    Set-MigrationBatch \<batchname>-ApproveSkippedItems 
2. ใช้คำสั่งต่อไปนี้เพื่ออนุมัติรายการที่ถูกข้ามในการร้องขอการโยกย้ายที่มี "ซิงค์" แต่ไม่เสร็จสมบูรณ์:

    $pf = ได้รับ PublicFolderMailboxMigrationRequest | ลี่ฟาน รับ-PublicFolderMailboxMigrationRequestStatistics-IncludeReport; ForEach ($i ใน $pf) {ถ้า ($i LargeItemsEncountered-gt 0-หรือ $i BadItemsEncountered-gt 0) {Set PublicFolderMailboxMigrationRequest $i รหัสประจำตัว IdentifyingGuid-SkippedItemApprovalTime ([DateTime]:: UtcNow)}}
3. แบทช์การโยกย้ายและการร้องขอควรดำเนินต่อและเสร็จสมบูรณ์ในไม่กี่นาที

