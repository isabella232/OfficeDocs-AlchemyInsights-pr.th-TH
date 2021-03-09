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
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>ข้อผิดพลาดที่อยู่พร็อกซีขณะสร้างกล่องจดหมายหรือวัตถุอีเมลอื่นที่เปิดใช้งาน

ถ้าคุณพยายามสร้างวัตถุที่เปิดใช้งานอีเมล (กล่องจดหมาย กล่องจดหมายที่แชร์ และอื่นๆ) และได้รับข้อผิดพลาด "ที่อยู่พร็อกซี "SMTP:alias@domain.com" ถูกใช้แล้ว..." ที่อยู่อีเมลที่คุณเลือกจะถูกถ่ายโดยวัตถุที่เปิดใช้งานอีเมลอื่นในองค์กรของคุณ
  
คุณต้องค้นหาผู้ใช้ กลุ่ม กล่องจดหมายที่แชร์ หรือโฟลเดอร์สาธารณะที่มีที่อยู่อีเมลนี้ และลบหรือเปลี่ยนที่อยู่อีเมล จากนั้นคุณสามารถสร้างวัตถุที่เปิดใช้งานอีเมลใหม่ด้วยที่อยู่อีเมลฟรี ใช้ ค้นหา บนหน้าแรกเพื่อค้นหา You can also use the following Exchange Online PowerShell command to search for it:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
ถ้าคุณไม่ต้องการลบที่อยู่อีเมลที่มีอยู่ ให้เลือกที่อยู่อีเมลใหม่ให้กับวัตถุใหม่ที่คุณสร้าง
  