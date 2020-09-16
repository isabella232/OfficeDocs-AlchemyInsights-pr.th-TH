---
title: จัดการผู้ใช้ที่ซิงโครไนซ์
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777696"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="c6b6d-102">ไม่สามารถตั้งค่าที่อยู่อีเมลหลักเปลี่ยนแอตทริบิวต์ของผู้ใช้หรือลบ/ลบผู้ใช้ที่ซิงโครไนซ์ได้</span><span class="sxs-lookup"><span data-stu-id="c6b6d-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="c6b6d-103">ถ้ามีการเปิดใช้งานการซิงโครไนซ์ไดเรกทอรีสำหรับสภาพแวดล้อมของคุณคุณจะไม่สามารถเปลี่ยนแอตทริบิวต์บางอย่างของผู้ใช้หรือวัตถุได้โดยใช้ศูนย์การจัดการ Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="c6b6d-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="c6b6d-104">เมื่อต้องการจัดการผู้ใช้ที่ซิงโครไนซ์และแอตทริบิวต์ทั้งหมดโดยสมบูรณ์ให้ใช้ผู้ใช้ของไดเรกทอรีที่ใช้งานอยู่ภายในเครื่องของคุณและคอนโซลการจัดการกลุ่ม (adsiedit. msc)</span><span class="sxs-lookup"><span data-stu-id="c6b6d-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="c6b6d-105">อีกวิธีหนึ่งคือคุณสามารถเปลี่ยนผู้ใช้แต่ละรายหรือแอตทริบิวต์สำหรับผู้ใช้ที่ทำข้อมูลให้ตรงกันโดยใช้ powershell เช่นที่แสดงในตัวอย่างทั่วไปเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="c6b6d-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
