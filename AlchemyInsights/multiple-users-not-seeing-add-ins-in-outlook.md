---
title: ผู้ใช้หลายคนไม่เห็น Add-in ใน Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198244"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="29d93-102">ผู้ใช้หลายคนไม่เห็น Add-in ใน Outlook</span><span class="sxs-lookup"><span data-stu-id="29d93-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="29d93-103">ถ้าคุณทดสอบโปรแกรม Outlook add-in และ none ปรากฏขึ้น เป็นขั้นตอนการแก้ไขปัญหาแรก ใช้ cmdlet รับ**OrganizationConfig** PowerShell การสอบถามพารามิเตอร์_AppsForOfficeEnabled_</span><span class="sxs-lookup"><span data-stu-id="29d93-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="29d93-104">ถ้าแบบสอบถามส่งกลับค่า**ของเท็จ**ตั้งค่าพารามิเตอร์นี้เป็น**Truy**โดยใช้ cmdlet **Set-OrganizationConfig**ดังนั้น add-ins ปรากฏตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="29d93-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="29d93-105">เราไม่แนะนําให้พารามิเตอร์_AppsForOfficeEnabled_ถูกตั้งค่าเป็น**เท็จ**</span><span class="sxs-lookup"><span data-stu-id="29d93-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="29d93-106">ค่าของ**False**จะแทนที่การตั้งค่าบทบาทผู้ดูแลระบบและผู้ใช้ข้างต้นทั้งหมด และป้องกันไม่ให้ผู้ใช้ใด ๆ ในองค์กรเปิดใช้งานแอปใหม่</span><span class="sxs-lookup"><span data-stu-id="29d93-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="29d93-107">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การระบุผู้ดูแลระบบและผู้ใช้ที่สามารถติดตั้งและจัดการ Add-in สําหรับ Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)</span><span class="sxs-lookup"><span data-stu-id="29d93-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>