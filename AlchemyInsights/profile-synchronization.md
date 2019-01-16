---
title: ซิงโครไนส์ส่วนกำหนดค่า
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28316548"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="120a9-102">เมื่อทำการเปลี่ยนแปลงส่วนกำหนดค่าของฉันซิงค์กับ SharePoint ใช้โปรไฟล์ผู้ใช้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="120a9-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="120a9-103">ออนไลน์ของ SharePoint ใช้งานตัวจับเวลาที่นำเข้าไดเรกทอรีที่ใช้งานอยู่ (นำเข้าโฆษณา) การนำเข้าผู้ใช้และกลุ่มในโปรไฟล์ผู้ใช้นี้</span><span class="sxs-lookup"><span data-stu-id="120a9-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="120a9-p101">นำเข้าโฆษณาซิงค์การเปลี่ยนแปลงจากเก็บ SharePoint ออนไลน์ไดเรกทอรีโปรไฟล์ผู้ใช้ การเปลี่ยนแปลงเหล่านี้จะถูกประมวลผลชุดงาน</span><span class="sxs-lookup"><span data-stu-id="120a9-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="120a9-106">งานตัวจับเวลาทำงานจนกว่ามีการเปลี่ยนแปลงจะถูกทำข้อมูลให้ตรงกัน</span><span class="sxs-lookup"><span data-stu-id="120a9-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="120a9-p102">เวลาใช้ในงานที่จะรันขึ้นอยู่กับจำนวนของการประมวลผลการเปลี่ยนแปลง เปลี่ยนแปลงเป็นจำนวนมากใช้เวลานานขึ้น ข้อตกลงระดับบริการ (SLA) ระบุว่า ผู้ใช้ในไดเรกทอรีออนไลน์ของ SharePoint การเปลี่ยนแปลงจะมีผลต่อโปรไฟล์ผู้ใช้ใน 24 ชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="120a9-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="120a9-110">รายละเอียดเพิ่มเติมเกี่ยวกับการซิงค์โพรไฟล์ผู้ใช้ใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="120a9-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

