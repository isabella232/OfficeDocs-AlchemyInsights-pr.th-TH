---
title: แก้ไขปัญหาการตั้งค่า DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744969"
---
# <a name="fix-dkim-setup-issues"></a>แก้ไขปัญหาการตั้งค่า DKIM

ถ้าคุณประสบปัญหาในการเปิดใช้งาน DKIM สำหรับโดเมนแบบกำหนดเองของคุณให้ทำตามขั้นตอนต่อไปนี้:

- ปัญหาการตั้งค่า DKIM ส่วนใหญ่จะเกี่ยวข้องกับระเบียน DNS ที่ไม่ถูกต้อง ตรวจสอบระเบียน CNAME ของ DKIM (**ไม่ใช่** ระเบียน TXT) ถูกจัดรูปแบบอย่างถูกต้อง สำหรับข้อมูลเพิ่มเติมให้ดู [หัวข้อ](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)นี้

- หลังจากที่คุณสร้างหรืออัปเดตระเบียน DNS DKIM ของคุณที่บริการโฮสต์ DNS สำหรับโดเมนของคุณ (โดยทั่วไปแล้วบริษัทจดทะเบียนโดเมนของคุณ) ให้รอระเบียน DNS เพื่อเผยแพร่

- ถ้าคุณไม่สามารถสร้างเรกคอร์ด DNS DKIM ในศูนย์การจัดการได้คุณสามารถแทน \<CustomDomain\> ที่ด้วยโดเมนแบบกำหนดเองของคุณ (ตัวอย่างเช่น contoso.com) และเรียกใช้คำสั่งนี้ใน[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`
