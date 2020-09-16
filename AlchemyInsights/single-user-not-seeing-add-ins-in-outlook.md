---
title: ผู้ใช้คนเดียวไม่เห็น add-in ใน Outlook
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
ms.openlocfilehash: 8c99b443a2d83f3ac24362d63cd6363a66a81393
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719684"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="6d8a6-102">ผู้ใช้คนเดียวไม่เห็น add-in ใน Outlook</span><span class="sxs-lookup"><span data-stu-id="6d8a6-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="6d8a6-103">ผู้ใช้อาจเป็นส่วนหนึ่งของบทบาทที่ไม่มีพารามิเตอร์ AppsForOfficeEnabled ที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="6d8a6-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="6d8a6-104">เรียกใช้ cmdlet นี้เพื่อค้นหาว่าบทบาทที่ถูกต้องเกี่ยวข้องกับผู้ใช้:</span><span class="sxs-lookup"><span data-stu-id="6d8a6-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="6d8a6-105">Get-ManagementRoleAssignment-RoleAssignee user@domain.com-การมอบ $false รูปแบบ-ตาราง-บทบาทอัตโนมัติ, RoleAssigneeName, RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="6d8a6-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="6d8a6-106">สำหรับข้อมูลเพิ่มเติมให้ดู [ที่ระบุผู้ดูแลระบบและผู้ใช้ที่สามารถติดตั้งและจัดการ add-in สำหรับ Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)ได้</span><span class="sxs-lookup"><span data-stu-id="6d8a6-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
