---
title: ชุดการโยกย้ายโฟลเดอร์สาธารณะไม่เสร็จสมบูรณ์แสดงการซิงค์
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
ms.openlocfilehash: 33302110249b02aef87639792ebfd9cafd6638c0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47804282"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="92d23-102">ชุดการโยกย้ายโฟลเดอร์สาธารณะไม่เสร็จสมบูรณ์แสดงการซิงค์</span><span class="sxs-lookup"><span data-stu-id="92d23-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="92d23-103">คุณอาจเริ่มการทำงานของชุดการโยกย้ายและสถานะของชุดการโยกย้ายต่อเนื่องแสดงว่า "ซิงค์" เป็นเวลานานมาก</span><span class="sxs-lookup"><span data-stu-id="92d23-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="92d23-104">นี่คือลักษณะการทำงานที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="92d23-104">This is expected behavior.</span></span>

<span data-ttu-id="92d23-105">โดยทั่วไปสำหรับสถานะของชุดการโยกย้ายจะยังคงอยู่ในการซิงค์ชั่วครู่ก่อนที่จะสลับไปยังการดำเนินการเสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="92d23-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="92d23-106">สำหรับการโยกย้ายที่เกี่ยวข้องกับกล่องจดหมายเป้าหมายจำนวนมากเป็นเรื่องปกติที่จะดูสถานะจะยังคงอยู่ในสถานะที่ซิงค์มานานกว่า24ชั่วโมงซึ่งไม่มีการร้องขอการโยกย้ายโฟลเดอร์สาธารณะที่อยู่ภายใต้ล้มเหลวหรือถูกกักกัน</span><span class="sxs-lookup"><span data-stu-id="92d23-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="92d23-107">โปรดอนุญาตให้24-48 ชั่วโมงสำหรับชุดการโยกย้ายเพื่อทำงานให้เสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="92d23-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>
