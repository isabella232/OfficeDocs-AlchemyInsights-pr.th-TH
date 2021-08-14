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
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062927"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>ข้อผิดพลาดที่อยู่พร็อกซีขณะสร้างกล่องจดหมายหรือวัตถุที่เปิดใช้งานอีเมลอื่นๆ

ถ้าคุณพยายามสร้างวัตถุที่เปิดใช้งานอีเมล (กล่องจดหมาย กล่องจดหมายที่แชร์ และอื่นๆ) และได้รับข้อผิดพลาด "มีการใช้ที่อยู่พร็อกซี "SMTP:alias@domain.com" ที่อยู่อีเมลที่คุณเลือกไว้แล้วโดยวัตถุที่เปิดใช้งานอีเมลอื่นในองค์กรของคุณ
  
คุณ need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address. จากนั้นคุณสามารถสร้างวัตถุใหม่ที่เปิดใช้งานอีเมลด้วยที่อยู่อีเมลฟรี ใช้ ค้นหา บน โฮมเพจ เพื่อค้นหา คุณยังสามารถใช้รายการต่อไปนี้Exchange Onlineสั่ง PowerShell เพื่อค้นหาได้:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
ถ้าคุณไม่ต้องการลบที่อยู่อีเมลที่มีอยู่ ให้เลือกที่อยู่อีเมลใหม่ให้กับวัตถุใหม่ที่คุณสร้าง
  