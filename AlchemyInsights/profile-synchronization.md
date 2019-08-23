---
title: ซิงโครไนส์ส่วนกำหนดค่า
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554352"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="73a71-102">เมื่อทำการเปลี่ยนแปลงส่วนกำหนดค่าของฉันซิงค์กับ SharePoint ใช้โปรไฟล์ผู้ใช้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="73a71-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="73a71-103">ออนไลน์ของ SharePoint ใช้งานตัวจับเวลาที่นำเข้าไดเรกทอรีที่ใช้งานอยู่ (นำเข้าโฆษณา) การนำเข้าผู้ใช้และกลุ่มในโปรไฟล์ผู้ใช้นี้</span><span class="sxs-lookup"><span data-stu-id="73a71-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="73a71-104">นำเข้าโฆษณาซิงค์การเปลี่ยนแปลงจากเก็บ SharePoint ออนไลน์ไดเรกทอรีโปรไฟล์ผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="73a71-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="73a71-105">การเปลี่ยนแปลงเหล่านี้จะถูกประมวลผลชุดงาน</span><span class="sxs-lookup"><span data-stu-id="73a71-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="73a71-106">งานตัวจับเวลาทำงานจนกว่ามีการเปลี่ยนแปลงจะถูกทำข้อมูลให้ตรงกัน</span><span class="sxs-lookup"><span data-stu-id="73a71-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="73a71-107">เวลาใช้ในงานที่จะรันขึ้นอยู่กับจำนวนของการประมวลผลการเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="73a71-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="73a71-108">เปลี่ยนแปลงเป็นจำนวนมากใช้เวลานานขึ้น</span><span class="sxs-lookup"><span data-stu-id="73a71-108">A large number of changes takes longer.</span></span> <span data-ttu-id="73a71-109">ข้อตกลงระดับบริการ (SLA) ระบุว่า ผู้ใช้ในไดเรกทอรีออนไลน์ของ SharePoint การเปลี่ยนแปลงจะมีผลต่อโปรไฟล์ผู้ใช้ใน 24 ชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="73a71-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="73a71-110">รายละเอียดเพิ่มเติมเกี่ยวกับการซิงค์โพรไฟล์ผู้ใช้ใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="73a71-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

