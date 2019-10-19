---
title: การซิงโครไนส์โปรไฟล์
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554352"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="6e0b4-102">โปรไฟล์ของฉันจะเปลี่ยนแปลงการซิงค์กับโปรแกรมประยุกต์ส่วนกำหนดค่าผู้ใช้ของ SharePoint เมื่อใด</span><span class="sxs-lookup"><span data-stu-id="6e0b4-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="6e0b4-103">SharePoint แบบออนไลน์ใช้งานตัวจับเวลาการนำเข้าไดเรกทอรีที่ใช้งานอยู่ (การนำเข้าโฆษณา) เพื่อนำเข้าผู้ใช้และกลุ่มไปยังโปรแกรมประยุกต์ส่วนกำหนดค่าผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="6e0b4-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="6e0b4-104">นำเข้าโฆษณาซิงค์การเปลี่ยนแปลงจากที่เก็บไดเรกทอรีแบบออนไลน์ของ SharePoint ไปยังโปรแกรมประยุกต์ส่วนกำหนดค่าผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="6e0b4-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="6e0b4-105">การเปลี่ยนแปลงเหล่านี้จะถูกประมวลผลเป็นชุดงาน</span><span class="sxs-lookup"><span data-stu-id="6e0b4-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="6e0b4-106">งานตัวจับเวลาจะรันจนกว่าจะมีการซิงค์การเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="6e0b4-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="6e0b4-107">เวลาที่ใช้งานในการรันจะขึ้นอยู่กับจำนวนของการเปลี่ยนแปลงที่จะประมวลผล</span><span class="sxs-lookup"><span data-stu-id="6e0b4-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="6e0b4-108">จำนวนมากของการเปลี่ยนแปลงจะใช้เวลานานกว่า</span><span class="sxs-lookup"><span data-stu-id="6e0b4-108">A large number of changes takes longer.</span></span> <span data-ttu-id="6e0b4-109">ข้อตกลงระดับการให้บริการ (SLA) ระบุว่าการเปลี่ยนแปลงผู้ใช้ในไดเรกทอรีแบบออนไลน์ของ SharePoint จะมีผลในแอพลิเคชันส่วนกำหนดค่าผู้ใช้ใน24ชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="6e0b4-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="6e0b4-110">ข้อมูลเพิ่มเติมเกี่ยวกับการซิงค์โพรไฟล์ผู้ใช้ใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="6e0b4-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

