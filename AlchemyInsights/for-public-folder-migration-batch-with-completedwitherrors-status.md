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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="f213f-102">สำหรับชุดงานการโยกย้ายโฟลเดอร์สาธารณะที่มีสถานะ CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="f213f-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="f213f-103">ใช้ขั้นตอนต่อไปนี้เพื่อทำให้ชุดงานการข้ามรายการขนาดใหญ่/ไม่ถูกต้อง:</span><span class="sxs-lookup"><span data-stu-id="f213f-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="f213f-104">อนุมัติรายการที่ถูกข้ามในแบทช์การย้าย:</span><span class="sxs-lookup"><span data-stu-id="f213f-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="f213f-105">Set-MigrationBatch \<batchname>-ApproveSkippedItems</span><span class="sxs-lookup"><span data-stu-id="f213f-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="f213f-106">ใช้คำสั่งต่อไปนี้เพื่ออนุมัติรายการที่ถูกข้ามในการร้องขอการโยกย้ายที่มี "ซิงค์" แต่ไม่เสร็จสมบูรณ์:</span><span class="sxs-lookup"><span data-stu-id="f213f-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="f213f-107">$pf = ได้รับ PublicFolderMailboxMigrationRequest | ลี่ฟาน รับ-PublicFolderMailboxMigrationRequestStatistics-IncludeReport; ForEach ($i ใน $pf) {ถ้า ($i LargeItemsEncountered-gt 0-หรือ $i BadItemsEncountered-gt 0) {Set PublicFolderMailboxMigrationRequest $i รหัสประจำตัว IdentifyingGuid-SkippedItemApprovalTime ([DateTime]:: UtcNow)}}</span><span class="sxs-lookup"><span data-stu-id="f213f-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="f213f-108">แบทช์การโยกย้ายและการร้องขอควรดำเนินต่อและเสร็จสมบูรณ์ในไม่กี่นาที</span><span class="sxs-lookup"><span data-stu-id="f213f-108">The migration batch and requests should resume and complete in a few minutes.</span></span>

