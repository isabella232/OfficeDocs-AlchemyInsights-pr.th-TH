---
title: การเข้าถึงถูกปฏิเสธเมื่อดูลำดับงาน
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36747767"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="c6fb0-102">การเข้าถึงถูกปฏิเสธเมื่อดูลำดับงาน</span><span class="sxs-lookup"><span data-stu-id="c6fb0-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="c6fb0-103">SharePoint ๒๐๑๓เวิร์กโฟลว์ที่พยายามส่งเมลไปยังกลุ่ม SharePoint สามารถล้มเหลวด้วยข้อผิดพลาด "การเข้าถึงถูกปฏิเสธ" ถ้าเป็นสมาชิกของกลุ่ม SharePoint ไม่ได้ตั้งค่าให้ทุกคน</span><span class="sxs-lookup"><span data-stu-id="c6fb0-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="c6fb0-104">**ในการแก้ไขปัญหานี้ให้ทำตามขั้นตอนเหล่านี้:**</span><span class="sxs-lookup"><span data-stu-id="c6fb0-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="c6fb0-105">อนุญาตให้ทุกคนดูสมาชิกของกลุ่ม SharePoint ได้</span><span class="sxs-lookup"><span data-stu-id="c6fb0-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="c6fb0-106">เอากลุ่ม SharePoint ออกจากบรรทัดถึงหรือ CC ของเมล</span><span class="sxs-lookup"><span data-stu-id="c6fb0-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="c6fb0-107">เพิ่มผู้ใช้ลงในบรรทัดถึงหรือสำเนาถึงอย่างชัดเจนถ้าไม่สามารถเปลี่ยนการมองเห็นเป็นสมาชิกสำหรับกลุ่ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="c6fb0-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="c6fb0-108">หากต้องการดูรายละเอียดเพิ่มเติมโปรดดูที่ HTTP ที่ไม่ได้รับ[อนุญาตให้/_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="c6fb0-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  