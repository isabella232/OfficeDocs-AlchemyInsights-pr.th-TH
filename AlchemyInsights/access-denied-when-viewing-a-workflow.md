---
title: การเข้าถึงถูกปฏิเสธเมื่อดูลำดับงาน
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050544"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="595bc-102">การเข้าถึงถูกปฏิเสธเมื่อดูลำดับงาน</span><span class="sxs-lookup"><span data-stu-id="595bc-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="595bc-103">SharePoint ๒๐๑๓เวิร์กโฟลว์ที่พยายามส่งเมลไปยังกลุ่ม SharePoint สามารถล้มเหลวด้วยข้อผิดพลาด "การเข้าถึงถูกปฏิเสธ" ถ้าเป็นสมาชิกของกลุ่ม SharePoint ไม่ได้ตั้งค่าให้ทุกคน</span><span class="sxs-lookup"><span data-stu-id="595bc-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="595bc-104">**ในการแก้ไขปัญหานี้ให้ทำตามขั้นตอนเหล่านี้:**</span><span class="sxs-lookup"><span data-stu-id="595bc-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="595bc-105">อนุญาตให้ทุกคนดูสมาชิกของกลุ่ม SharePoint ได้</span><span class="sxs-lookup"><span data-stu-id="595bc-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="595bc-106">เอากลุ่ม SharePoint ออกจากบรรทัดถึงหรือ CC ของเมล</span><span class="sxs-lookup"><span data-stu-id="595bc-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="595bc-107">เพิ่มผู้ใช้ลงในบรรทัดถึงหรือสำเนาถึงอย่างชัดเจนถ้าไม่สามารถเปลี่ยนการมองเห็นเป็นสมาชิกสำหรับกลุ่ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="595bc-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="595bc-108">หากต้องการดูรายละเอียดเพิ่มเติมโปรดดูที่ HTTP ที่ไม่ได้รับ[อนุญาต/_vti_bin/client.svc/sp.utilities.utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="595bc-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  