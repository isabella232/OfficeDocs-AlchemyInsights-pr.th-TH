---
title: จัดการผู้ใช้ให้ตรงกัน
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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380524"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="f03e5-102">ไม่สามารถกำหนดที่อยู่อีเมลหลัก หรือเปลี่ยนแอตทริบิวต์ของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="f03e5-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="f03e5-103">ถ้าเปิดใช้งานการซิงโครไนส์ของไดเรกทอรีสำหรับสภาพแวดล้อมของคุณ บางแอตทริบิวต์ผู้ใช้หรือวัตถุที่ไม่สามารถเปลี่ยนใช้ศูนย์ดูแล</span><span class="sxs-lookup"><span data-stu-id="f03e5-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="f03e5-104">เมื่อต้องการจัดการผู้ใช้ให้ตรงกันและคุณลักษณะทั้งหมดของทั้งหมด ใช้ของไดเรกทอรีที่ใช้งานอยู่ภายในเครื่องผู้ใช้และกลุ่มคอนโซลการจัดการ (adsiedit.msc)</span><span class="sxs-lookup"><span data-stu-id="f03e5-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="f03e5-105">อีกวิธีหนึ่งคือ คุณสามารถเปลี่ยนแปลงแต่ละคนหรือแอตทริบิวต์สำหรับผู้ใช้ให้ตรงกันโดยใช้ powershell ที่แสดงในตัวอย่างเหล่านี้ทั่วไปเช่น:</span><span class="sxs-lookup"><span data-stu-id="f03e5-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="f03e5-106">การ user2@yourvanitydomain.onmicrosoft.com - AlternateEmailAddresses user@yourdomain.onmicrosoft.com - UserPrincipalName ชุด MsolUser</span><span class="sxs-lookup"><span data-stu-id="f03e5-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="f03e5-107">ชุด-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "ผู้ใช้ทดสอบ" - เขตข้อมูล LastName "ผู้ใช้" - "ผู้จัดการ" ชื่อเรื่อง-แผนก "ทรัพยากรบุคคล"</span><span class="sxs-lookup"><span data-stu-id="f03e5-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="f03e5-108">เอา-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="f03e5-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>