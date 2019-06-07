---
title: แก้ไขปัญหาการตั้งค่าของ DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765483"
---
# <a name="fix-dkim-setup-issues"></a>แก้ไขปัญหาการตั้งค่าของ DKIM

ถ้าคุณประสบปัญหาในการเปิดใช้งาน DKIM สำหรับโดเมนของคุณเอง ให้ใช้ขั้นตอนต่อไปนี้:

- ปัญหาการตั้งค่า DKIM ส่วนใหญ่เกี่ยวข้องกับระเบียน DNS ที่ไม่ถูกต้อง ตรวจสอบระเบียน DKIM CNAME (**ไม่**เรกคอร์ด TXT) ถูกจัดรูปแบบอย่างถูกต้อง สำหรับข้อมูลเพิ่มเติม ให้ดู[หัวข้อ](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)นี้

- หลังจากที่คุณสร้าง หรือปรับปรุงระเบียน DKIM DNS ของคุณใน DNS โฮสต์การบริการสำหรับโดเมนของคุณ (โดยทั่วไป ของโดเมนผู้ลงทะเบียน) รอสำหรับระเบียน DNS ที่จะเผยแพร่

- ถ้าคุณไม่สามารถสร้าง DKIM DNS ระเบียนใน admin ศูนย์ คุณสามารถแทน\<CustomDomain\>กับโดเมนของคุณเอง (ตัวอย่างเช่น contoso.com) และเรียกใช้คำสั่งนี้ใน[PowerShell ออนไลน์ของ Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):`New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`ได้
