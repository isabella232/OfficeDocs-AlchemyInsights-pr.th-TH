---
title: วิธีแก้ปัญหาสำหรับข้อผิดพลาด 30016-4
ms.author: janellem
author: janellem
manager: scotv
ms.date: 12/19/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 21644564-4ba5-4537-abd3-9ac2dfe2ee47
ms.openlocfilehash: 38079f76eb410592e48d93409e705faa9788fe19
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28316975"
---
# <a name="solutions-for-error-30016-4"></a><span data-ttu-id="2da92-102">วิธีแก้ปัญหาสำหรับข้อผิดพลาด 30016-4</span><span class="sxs-lookup"><span data-stu-id="2da92-102">Solutions for error 30016-4</span></span>

<span data-ttu-id="2da92-103">เมื่อคุณพยายามถอนการติดตั้ง Office 365 ProPlus จากคอมพิวเตอร์ คุณอาจได้รับข้อความแสดงข้อผิดพลาดต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="2da92-103">When you try to uninstall Office 365 ProPlus from a computer, you might receive the following error message:</span></span>
  
> <span data-ttu-id="2da92-104">"บางสิ่งบางอย่างไป 4 30016 ที่ไม่ถูกต้อง"</span><span class="sxs-lookup"><span data-stu-id="2da92-104">"Something went wrong 30016-4"</span></span>
    
<span data-ttu-id="2da92-105">ปัญหานี้เกิดขึ้นถ้าไดรฟ์ **% temp %** ถูกแมปไปยังไดรฟ์อื่นที่ไม่ใช่ **% ProgramFiles %**</span><span class="sxs-lookup"><span data-stu-id="2da92-105">This issue occurs if the **%temp%** drive is mapped to a drive other than **%ProgramFiles%**.</span></span> 
  
<span data-ttu-id="2da92-106">เมื่อต้องการแก้ไข เอา Office จากคอมพิวเตอร์</span><span class="sxs-lookup"><span data-stu-id="2da92-106">To fix, completely remove Office from the computer.</span></span>
  
1. <span data-ttu-id="2da92-107">ดาวน์โหลด และติดตั้งการ[สนับสนุนและผู้ช่วยกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="2da92-107">Download and install the [Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy).</span></span>
    
2. <span data-ttu-id="2da92-108">เมื่อเปิด จาก**ผลิตภัณฑ์การถอนการติดตั้ง Office**ให้เลือกรุ่นคุณต้องการถอนการติดตั้ง และเลือก**ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="2da92-108">When it opens, from **Uninstall Office products** select the version you want to uninstall and select **Next**.</span></span> 
    
3. <span data-ttu-id="2da92-109">ดำเนินต่อผ่านหน้าจอ และรีสตาร์ทเครื่องคอมพิวเตอร์เมื่อได้รับพร้อมท์</span><span class="sxs-lookup"><span data-stu-id="2da92-109">Continue going through screens and restart your computer when prompted.</span></span>
    
    <span data-ttu-id="2da92-110">หลังจากเริ่มการทำงาน การสนับสนุนและผู้ช่วยกู้คืนอีกครั้งเปิดโดยอัตโนมัติเพื่อให้การถอนการติดตั้งเสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="2da92-110">After restarting, the Support and Recovery Assistant automatically re-opens to complete the uninstall process.</span></span>
    
4. <span data-ttu-id="2da92-111">ทำตามตามพร้อมท์ที่เหลือ และติดตั้ง Office หรือปิดผู้ช่วย</span><span class="sxs-lookup"><span data-stu-id="2da92-111">Follow remaining prompts, and reinstall Office or close the assistant.</span></span>
    

