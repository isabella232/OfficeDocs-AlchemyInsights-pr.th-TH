---
title: ผู้ใช้หลายคนไม่เห็น add-in ใน Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729890"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="ae2c7-102">ผู้ใช้หลายคนไม่เห็น add-in ใน Outlook</span><span class="sxs-lookup"><span data-stu-id="ae2c7-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="ae2c7-103">ถ้าคุณทดสอบ add-in ของ Outlook และไม่มีการแสดงเป็นขั้นตอนการแก้ไขปัญหาแรกให้ใช้ cmdlet PowerShell**ชื่อ get-organizationconfig**เพื่อสอบถามพารามิเตอร์_AppsForOfficeEnabled_</span><span class="sxs-lookup"><span data-stu-id="ae2c7-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="ae2c7-104">ถ้าคิวรีส่งกลับค่า **False**ให้ตั้งค่าพารามิเตอร์นี้เป็น **True** โดยใช้ Cmdlet การ **ตั้งค่าชื่อ get-organizationconfig** ดังนั้น add-in จะปรากฏขึ้นตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="ae2c7-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="ae2c7-105">เราไม่แนะนำให้พารามิเตอร์_AppsForOfficeEnabled_ถูกตั้งค่าเป็น**False**</span><span class="sxs-lookup"><span data-stu-id="ae2c7-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="ae2c7-106">ค่าของ **False** จะแทนที่การตั้งค่าบทบาทของผู้ดูแลระบบและผู้ใช้ทั้งหมดและป้องกันไม่ให้แอปใหม่ถูกเปิดใช้งานโดยผู้ใช้ใดๆในองค์กร</span><span class="sxs-lookup"><span data-stu-id="ae2c7-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="ae2c7-107">สำหรับข้อมูลเพิ่มเติมให้ดู [ที่ระบุผู้ดูแลระบบและผู้ใช้ที่สามารถติดตั้งและจัดการ add-in สำหรับ Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)ได้</span><span class="sxs-lookup"><span data-stu-id="ae2c7-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>