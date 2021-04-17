---
title: เหตุการณ์ในปฏิทินหายไปหรือไม่อัปเดต
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837588"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="6c5db-102">เหตุการณ์ในปฏิทินหายไปหรือไม่อัปเดต</span><span class="sxs-lookup"><span data-stu-id="6c5db-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="6c5db-103">ถ้ารายการปฏิทินหายไปหรือไม่อัปเดต ให้เริ่มต้นโดยการดูที่การนับรายการในคุณสมบัติโฟลเดอร์ปฏิทินใน Outlook:</span><span class="sxs-lookup"><span data-stu-id="6c5db-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="6c5db-104">คลิกขวาที่โฟลเดอร์ **ปฏิทิน** ของผู้ใช้ที่ได้รับผลกระทบ **แล้วเลือก** คุณสมบัติ</span><span class="sxs-lookup"><span data-stu-id="6c5db-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="6c5db-105">เลือก **แท็บ** การซิงโครไนซ์</span><span class="sxs-lookup"><span data-stu-id="6c5db-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="6c5db-106">ถ้าการนับรายการไม่เหมือนกันระหว่างโฟลเดอร์เซิร์ฟเวอร์และโฟลเดอร์ออฟไลน์ ให้ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="6c5db-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="6c5db-107">ไฮไลต์ **โฟลเดอร์** ปฏิทิน</span><span class="sxs-lookup"><span data-stu-id="6c5db-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="6c5db-108">ไปที่แท็บ / **ส่ง** และรับ แล้วเลือก **อัปเดต** โฟลเดอร์</span><span class="sxs-lookup"><span data-stu-id="6c5db-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="6c5db-109">ถ้าปฏิทินของคุณยังคงไม่อัปเดตหรือเหตุการณ์หายไป ให้ดาวน์โหลดเครื่องมือตรวจสอบปฏิทินของ Outlook จาก[ศูนย์ดาวน์โหลด Microsoft](https://www.microsoft.com/download/details.aspx?id=28786)</span><span class="sxs-lookup"><span data-stu-id="6c5db-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="6c5db-110">ตรวจสอบว่ามีรายการมากกว่า 5000 รายการในโฟลเดอร์ปฏิทินหรือไม่ เนื่องจากอาจทําให้เกิดอาการ เช่น การประชุมในปฏิทินไม่ได้รับการอัปเดตหรือข้อผิดพลาดการประชุม</span><span class="sxs-lookup"><span data-stu-id="6c5db-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="6c5db-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span><span class="sxs-lookup"><span data-stu-id="6c5db-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>