---
title: For Public folder migration batch with CompletedWithErrors status
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068183"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>For Public folder migration batch with CompletedWithErrors status

ใช้ขั้นตอนต่อไปนี้เพื่อเสร็จสิ้นชุดการข้ามรายการขนาดใหญ่/ไม่ดี: 
1. อนุมัติรายการที่ข้ามบนชุดการโยกย้าย:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. ใช้การสั่งต่อไปนี้เพื่ออนุมัติรายการที่ข้ามในการร้องขอการโยกย้ายที่เป็น "ซิงค์แล้ว" แต่ไม่เสร็จสมบูรณ์:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. ชุดการโยกย้ายและการร้องขอควรประวัติย่อและเสร็จสมบูรณ์ในอีกสักครู่

