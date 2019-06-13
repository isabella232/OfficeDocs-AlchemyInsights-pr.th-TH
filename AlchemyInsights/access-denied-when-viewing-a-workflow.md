---
title: การเข้าถึงถูกปฏิเสธเมื่อดูเวิร์กโฟลว์
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: b7a3805d30cac44781adbbb00c0f0ed3496ff17b
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/12/2019
ms.locfileid: "34883610"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="e37a3-102">การเข้าถึงถูกปฏิเสธเมื่อดูเวิร์กโฟลว์</span><span class="sxs-lookup"><span data-stu-id="e37a3-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="e37a3-103">SharePoint 2013 เวิร์กโฟลว์ที่พยายามที่จะส่งอีเมลไปยังกลุ่ม SharePoint สามารถล้มเหลว ด้วยข้อผิดพลาด "Access Denied" ถ้าเป็นสมาชิกของกลุ่ม SharePoint ไม่ได้ตั้งค่าเพื่อให้ทุกคน</span><span class="sxs-lookup"><span data-stu-id="e37a3-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="e37a3-104">**เมื่อต้องการแก้ไขปัญหานี้ ทำตามขั้นตอนเหล่านี้:**</span><span class="sxs-lookup"><span data-stu-id="e37a3-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="e37a3-105">อนุญาตให้ทุกคนเมื่อต้องการดูสมาชิกของกลุ่ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="e37a3-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="e37a3-106">เอากลุ่ม SharePoint จาก'ถึง'หรือ'สำเนาถึง'บรรทัดของอีเมลอยู่</span><span class="sxs-lookup"><span data-stu-id="e37a3-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="e37a3-107">เพิ่มผู้ใช้ไป'ถึง'หรือ'สำเนาถึง'อย่างชัดเจนบรรทัดหากคุณไม่สามารถเปลี่ยนการมองเห็นเป็นสมาชิกของกลุ่ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="e37a3-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="e37a3-108">เมื่อต้องการดู รายละเอียดเพิ่มเติมกรุณาอ้างอิง[HTTP ไม่ได้รับอนุญาตเพื่อ /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="e37a3-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  