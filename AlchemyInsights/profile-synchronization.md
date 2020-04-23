---
title: การซิงโครไนซ์โปรไฟล์
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768132"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="59ad9-102">โปรไฟล์ของฉันเปลี่ยนแปลงไปในโปรแกรมประยุกต์ SharePoint โปรไฟล์ผู้ใช้เมื่อใด</span><span class="sxs-lookup"><span data-stu-id="59ad9-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="59ad9-103">SharePoint แบบออนไลน์ใช้งานตัวจับเวลาการนําเข้าไดเรกทอรีที่ใช้งานอยู่ (นําเข้าโฆษณา) เพื่อนําเข้าผู้ใช้และกลุ่มลงในแอพลิเคชันส่วนกําหนดค่าผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="59ad9-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="59ad9-104">การนําเข้าโฆษณาซิงค์การเปลี่ยนแปลงจากที่เก็บไดเรกทอรีของ SharePoint แบบออนไลน์ไปยังโปรแกรมประยุกต์โปรไฟล์ผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="59ad9-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="59ad9-105">การเปลี่ยนแปลงเหล่านี้จะถูกประมวลผลในชุดงาน</span><span class="sxs-lookup"><span data-stu-id="59ad9-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="59ad9-106">งานตัวจับเวลารันจนกว่าการเปลี่ยนแปลงจะถูกทําข้อมูลให้ตรงกัน</span><span class="sxs-lookup"><span data-stu-id="59ad9-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="59ad9-107">เวลาที่งานนี้ใช้รันขึ้นอยู่กับจํานวนของการเปลี่ยนแปลงที่จะดําเนินการ</span><span class="sxs-lookup"><span data-stu-id="59ad9-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="59ad9-108">การเปลี่ยนแปลงจํานวนมากใช้เวลานานขึ้น</span><span class="sxs-lookup"><span data-stu-id="59ad9-108">A large number of changes takes longer.</span></span> <span data-ttu-id="59ad9-109">ข้อตกลงระดับการให้บริการ (SLA) ระบุว่า การเปลี่ยนแปลงไปยังผู้ใช้ในไดเรกทอรีแบบออนไลน์ของ SharePoint จะสะท้อนในแอพลิเคชันส่วนกําหนดค่าผู้ใช้ใน 24 ชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="59ad9-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="59ad9-110">ข้อมูลเพิ่มเติมเกี่ยวกับการซิงค์โพรไฟล์ผู้ใช้ใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="59ad9-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

