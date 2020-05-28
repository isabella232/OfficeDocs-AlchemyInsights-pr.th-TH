---
title: จัดการผู้ใช้ที่ซิงโครไนซ์
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407369"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="4bdbe-102">ไม่สามารถตั้งค่าที่อยู่อีเมลหลัก</span><span class="sxs-lookup"><span data-stu-id="4bdbe-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="4bdbe-103">ถ้าการซิงโครไนส์ของไดเรกทอรีถูกเปิดใช้งานสําหรับสภาพแวดล้อมของคุณ</span><span class="sxs-lookup"><span data-stu-id="4bdbe-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="4bdbe-104">ในการจัดการผู้ใช้ที่ซิงโครไนซ์และแอตทริบิวต์ทั้งหมดให้ใช้คอนโซลการจัดการไดเรกทอรีที่ใช้งานอยู่ในท้องถิ่นและกลุ่ม (adsiedit.msc)</span><span class="sxs-lookup"><span data-stu-id="4bdbe-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="4bdbe-105">อีกวิธีหนึ่งคือ คุณสามารถเปลี่ยนผู้ใช้หรือแอตทริบิวต์สําหรับผู้ใช้ที่ซิงโครไนซ์โดยใช้ powershell เช่นที่แสดงในตัวอย่างทั่วไปเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="4bdbe-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
