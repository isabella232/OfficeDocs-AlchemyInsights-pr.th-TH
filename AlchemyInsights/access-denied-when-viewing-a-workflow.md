---
title: การเข้าถึงถูกปฏิเสธเมื่อดูเวิร์กโฟลว์
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688821"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="e09c2-102">การเข้าถึงถูกปฏิเสธเมื่อดูเวิร์กโฟลว์</span><span class="sxs-lookup"><span data-stu-id="e09c2-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="e09c2-103">เวิร์กโฟลว์ SharePoint ๒๐๑๓ที่พยายามส่งอีเมลไปยังกลุ่ม SharePoint สามารถล้มเหลวโดยมีข้อความแสดงข้อผิดพลาด "การเข้าถึงถูกปฏิเสธ" ถ้าการเป็นสมาชิกของกลุ่ม SharePoint ไม่ได้ถูกตั้งค่าให้ทุกคน</span><span class="sxs-lookup"><span data-stu-id="e09c2-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="e09c2-104">**เมื่อต้องการแก้ไขปัญหานี้ให้ทำตามขั้นตอนต่อไปนี้:**</span><span class="sxs-lookup"><span data-stu-id="e09c2-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="e09c2-105">อนุญาตให้ทุกคนเห็นสมาชิกของกลุ่ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="e09c2-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="e09c2-106">เอากลุ่ม SharePoint ออกจากบรรทัดถึงหรือสำเนาถึงของอีเมล</span><span class="sxs-lookup"><span data-stu-id="e09c2-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="e09c2-107">เพิ่มผู้ใช้ลงในบรรทัดถึงหรือสำเนาถึงอย่างชัดเจนถ้าการมองเห็นเป็นสมาชิกไม่สามารถเปลี่ยนแปลงได้สำหรับกลุ่ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="e09c2-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="e09c2-108">เมื่อต้องการดูรายละเอียดเพิ่มเติมโปรดดูที่[HTTP ที่ไม่ได้รับอนุญาตให้เข้าถึง/_vti_bin/client.svc/sp.utilities.utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="e09c2-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  