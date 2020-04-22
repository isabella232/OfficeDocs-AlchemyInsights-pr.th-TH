---
title: การเข้าถึงถูกปฏิเสธเมื่อดูเวิร์กโฟลว์
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687349"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="782e4-102">การเข้าถึงถูกปฏิเสธเมื่อดูเวิร์กโฟลว์</span><span class="sxs-lookup"><span data-stu-id="782e4-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="782e4-103">SharePoint 2013 เวิร์กโฟลว์ที่พยายามส่งอีเมลไปยังกลุ่ม SharePoint สามารถล้มเหลว ด้วยข้อความข้อผิดพลาด "การเข้าถึงถูกปฏิเสธ"</span><span class="sxs-lookup"><span data-stu-id="782e4-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="782e4-104">**เมื่อต้องการแก้ไขปัญหานี้ ให้ทําตามขั้นตอนเหล่านี้:**</span><span class="sxs-lookup"><span data-stu-id="782e4-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="782e4-105">อนุญาตให้ทุกคนเห็นสมาชิกของกลุ่ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="782e4-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="782e4-106">เอากลุ่ม SharePoint จากบรรทัดถึงหรือสําเนาถึงของอีเมล</span><span class="sxs-lookup"><span data-stu-id="782e4-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="782e4-107">เพิ่มผู้ใช้ไปยังบรรทัดถึงหรือสําเนาถึงอย่างชัดเจนถ้าไม่สามารถเปลี่ยนแปลงการมองเห็นการเป็นสมาชิกสําหรับกลุ่ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="782e4-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="782e4-108">หากต้องการดูรายละเอียดเพิ่มเติม โปรดดูที่[HTTP ไม่ได้รับอนุญาตให้ /_vti_bin/client.svc/sp.utilities.utilities.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="782e4-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  