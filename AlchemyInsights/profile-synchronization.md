---
title: การซิงโครไนซ์โปรไฟล์
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801788"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="df788-102">เมื่อใดโปรไฟล์ของฉันจะเปลี่ยนการซิงค์ไปยังแอปพลิเคชันโปรไฟล์ผู้ใช้ SharePoint</span><span class="sxs-lookup"><span data-stu-id="df788-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="df788-103">SharePoint Online ใช้งานตัวจับเวลาการนำเข้าไดเรกทอรีที่ใช้งานอยู่ (การนำเข้าโฆษณา) เพื่อนำเข้าผู้ใช้และกลุ่มลงในแอปพลิเคชันโปรไฟล์ผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="df788-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="df788-104">การนำเข้าโฆษณาซิงโครไนซ์การเปลี่ยนแปลงจากที่เก็บไดเรกทอรี SharePoint Online ไปยังแอปพลิเคชันโปรไฟล์ผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="df788-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="df788-105">การเปลี่ยนแปลงเหล่านี้จะถูกประมวลผลในชุดงาน</span><span class="sxs-lookup"><span data-stu-id="df788-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="df788-106">งานตัวจับเวลาจะทำงานจนกว่าจะมีการซิงค์การเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="df788-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="df788-107">เวลาที่ใช้งานจะทำงานขึ้นอยู่กับจำนวนการเปลี่ยนแปลงที่จะดำเนินการ</span><span class="sxs-lookup"><span data-stu-id="df788-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="df788-108">มีการเปลี่ยนแปลงจำนวนมากใช้เวลานานขึ้น</span><span class="sxs-lookup"><span data-stu-id="df788-108">A large number of changes takes longer.</span></span> <span data-ttu-id="df788-109">ข้อตกลงระดับบริการ (SLA) ระบุว่าการเปลี่ยนแปลงไปยังผู้ใช้ในไดเรกทอรี SharePoint Online จะปรากฏในแอปพลิเคชันโปรไฟล์ผู้ใช้ใน24ชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="df788-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="df788-110">ข้อมูลเพิ่มเติมเกี่ยวกับการซิงค์โปรไฟล์ผู้ใช้ใน SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="df788-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

