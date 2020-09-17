---
title: การโยกย้ายโฟลเดอร์สาธารณะล้มเหลวที่๙๕%
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47803926"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="369db-102">การโยกย้ายโฟลเดอร์สาธารณะล้มเหลวที่๙๕%</span><span class="sxs-lookup"><span data-stu-id="369db-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="369db-103">คุณอาจเริ่มต้นชุดการโยกย้ายเสร็จสมบูรณ์แล้วและสถานะของชุดการโยกย้ายจะยังคงแสดงการ **ซิงค์** เป็นเวลานานมาก</span><span class="sxs-lookup"><span data-stu-id="369db-103">You might have initiated completion of a migration batch, and the status of the migration batch continues showing **Synced** for a very long time.</span></span> <span data-ttu-id="369db-104">นี่คือลักษณะการทำงานที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="369db-104">This is expected behavior.</span></span>

<span data-ttu-id="369db-105">โดยทั่วไปสำหรับสถานะของชุดการโยกย้ายจะยังคงอยู่ในการ**ซิงค์**ชั่วครู่ก่อนที่จะสลับไปยังการ**ดำเนินการเสร็จสมบูรณ์**</span><span class="sxs-lookup"><span data-stu-id="369db-105">It's common for the status of a migration batch to remain on **Synced** for a few hours before it switches to **Completing**.</span></span> <span data-ttu-id="369db-106">สำหรับการโยกย้ายที่เกี่ยวข้องกับกล่องจดหมายเป้าหมายจำนวนมากเป็นเรื่องปกติที่จะดูสถานะจะยังคงอยู่ในสถานะที่ซิงค์มานานกว่า24ชั่วโมงซึ่งไม่มีการร้องขอการโยกย้ายโฟลเดอร์สาธารณะที่อยู่ภายใต้ล้มเหลวหรือถูกกักกัน</span><span class="sxs-lookup"><span data-stu-id="369db-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="369db-107">โปรดอนุญาตให้24-48 ชั่วโมงสำหรับชุดการโยกย้ายเพื่อทำงานให้เสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="369db-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

<span data-ttu-id="369db-108">สำหรับการโยกย้ายโฟลเดอร์สาธารณะล้มเหลวที่๙๕% ที่มีข้อผิดพลาด FailedToMailEnablePublicFoldersException:</span><span class="sxs-lookup"><span data-stu-id="369db-108">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="369db-109">ดาวน์โหลดและเรียกใช้สคริปต์ [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) ที่เซิร์ฟเวอร์ Exchange ภายในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="369db-109">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="369db-110">ดำเนินการการดำเนินการแก้ไขที่แนะนำโดยสคริปต์</span><span class="sxs-lookup"><span data-stu-id="369db-110">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="369db-111">เรียกใช้การซิงค์-MailPublicFolders (สำหรับ Exchange ๒๐๑๐) หรือซิงค์-ModernMailPublicFolders (สำหรับ Exchange ๒๐๑๓และเวอร์ชันที่ใหม่กว่า)</span><span class="sxs-lookup"><span data-stu-id="369db-111">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="369db-112">ดำเนินการการโยกย้ายโฟลเดอร์สาธารณะต่อ</span><span class="sxs-lookup"><span data-stu-id="369db-112">Resume public folder migration.</span></span>
