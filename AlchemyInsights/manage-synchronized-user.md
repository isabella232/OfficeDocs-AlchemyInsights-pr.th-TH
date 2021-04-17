---
title: จัดการผู้ใช้ที่ซิงโครไนซ์
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823986"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="33de9-102">ไม่สามารถตั้งค่าที่อยู่อีเมลหลัก เปลี่ยนแอตทริบิวต์ของผู้ใช้ หรือลบผู้ใช้ที่ถูกซิงโครไนซ์</span><span class="sxs-lookup"><span data-stu-id="33de9-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="33de9-103">ถ้าเปิดใช้งานการซิงโครไนซ์ไดเรกทอรีกับสภาพแวดล้อมของคุณ แอตทริบิวต์ผู้ใช้หรือวัตถุบางอย่างจะไม่สามารถเปลี่ยนแปลงได้โดยใช้ศูนย์การจัดการ Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="33de9-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="33de9-104">เมื่อต้องการจัดการผู้ใช้ที่ซิงโครไนซ์และแอตทริบิวต์ทั้งหมดให้สมบูรณ์ ให้ใช้ผู้ใช้ไดเรกทอรีที่ใช้งานอยู่ภายในเครื่องและคอนโซลการจัดการกลุ่ม (adsiedit.msc)</span><span class="sxs-lookup"><span data-stu-id="33de9-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="33de9-105">อีกวิธีหนึ่งคือ คุณสามารถเปลี่ยนผู้ใช้แต่ละรายหรือแอตทริบิวต์ของผู้ใช้ที่ซิงโครไนซ์โดยใช้ Powershell เช่นที่แสดงในตัวอย่างทั่วไปเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="33de9-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
