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
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158643"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="b5728-102">สำหรับชุดงานการโยกย้ายโฟลเดอร์สาธารณะที่มีสถานะ CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="b5728-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="b5728-103">ใช้ขั้นตอนต่อไปนี้เพื่อทำให้ชุดงานการข้ามรายการขนาดใหญ่/ไม่ถูกต้อง:</span><span class="sxs-lookup"><span data-stu-id="b5728-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="b5728-104">อนุมัติรายการที่ถูกข้ามในแบทช์การย้าย:</span><span class="sxs-lookup"><span data-stu-id="b5728-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="b5728-105">ใช้คำสั่งต่อไปนี้เพื่ออนุมัติรายการที่ถูกข้ามในการร้องขอการโยกย้ายที่มี "ซิงค์" แต่ไม่เสร็จสมบูรณ์:</span><span class="sxs-lookup"><span data-stu-id="b5728-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="b5728-106">แบทช์การโยกย้ายและการร้องขอควรดำเนินต่อและเสร็จสมบูรณ์ในไม่กี่นาที</span><span class="sxs-lookup"><span data-stu-id="b5728-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

