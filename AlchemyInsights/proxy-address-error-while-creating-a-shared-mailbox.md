---
title: ข้อผิดพลาดที่อยู่พร็อกซีขณะสร้างกล่องจดหมายที่แชร์
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568309"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="2f6d6-102">ข้อผิดพลาดที่อยู่พร็อกซีขณะสร้างกล่องจดหมายหรือวัตถุอีเมลอื่นที่เปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="2f6d6-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="2f6d6-103">ถ้าคุณพยายามสร้างวัตถุที่เปิดใช้งานอีเมล (กล่องจดหมาย กล่องจดหมายที่แชร์ และอื่นๆ) และได้รับข้อผิดพลาด "ที่อยู่พร็อกซี "SMTP:alias@domain.com" ถูกใช้แล้ว..." ที่อยู่อีเมลที่คุณเลือกจะถูกถ่ายโดยวัตถุที่เปิดใช้งานอีเมลอื่นในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="2f6d6-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="2f6d6-104">คุณต้องค้นหาผู้ใช้ กลุ่ม กล่องจดหมายที่แชร์ หรือโฟลเดอร์สาธารณะที่มีที่อยู่อีเมลนี้ และลบหรือเปลี่ยนที่อยู่อีเมล</span><span class="sxs-lookup"><span data-stu-id="2f6d6-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="2f6d6-105">จากนั้นคุณสามารถสร้างวัตถุที่เปิดใช้งานอีเมลใหม่ด้วยที่อยู่อีเมลฟรี</span><span class="sxs-lookup"><span data-stu-id="2f6d6-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="2f6d6-106">ใช้ ค้นหา บนหน้าแรกเพื่อค้นหา</span><span class="sxs-lookup"><span data-stu-id="2f6d6-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="2f6d6-107">You can also use the following Exchange Online PowerShell command to search for it:</span><span class="sxs-lookup"><span data-stu-id="2f6d6-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="2f6d6-108">ถ้าคุณไม่ต้องการลบที่อยู่อีเมลที่มีอยู่ ให้เลือกที่อยู่อีเมลใหม่ให้กับวัตถุใหม่ที่คุณสร้าง</span><span class="sxs-lookup"><span data-stu-id="2f6d6-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  