---
title: แก้ไขปัญหาทั่วไปเกี่ยวกับการจัดรูปแบบระเบียน DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750754"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>แก้ไขปัญหาทั่วไปเกี่ยวกับการจัดรูปแบบระเบียน DKIM

ปัญหาการตั้งค่า DKIM ส่วนใหญ่เกี่ยวข้องกับระเบียน DNS ที่ไม่ถูกต้อง

เมื่อต้องการแก้ไขปัญหาการตั้งค่า DKIM ให้ตรวจสอบว่าระเบียน CNAME ของ DKIM **(ไม่ใช่** ระเบียน TXT) ได้รับการจัดรูปแบบอย่างถูกต้อง For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

ถ้าคุณต้องการความช่วยเหลือเกี่ยวกับระเบียน DNS โดยทั่วไป ให้ดูที่ สร้างระเบียน[DNS ที่ผู้ให้บริการโฮสต์ DNS ใดก็ได้ของ Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> หลังจากที่คุณสร้างหรืออัปเดตระเบียน DNS DKIM ของคุณที่บริการโฮสต์ DNS ให้กับโดเมนของคุณแล้ว คุณจะต้องรอให้ระเบียน DNS เผยแพร่
