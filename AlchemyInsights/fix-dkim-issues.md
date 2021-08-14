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
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945950"
---
# <a name="fix-dkim-setup-issues"></a>แก้ไขปัญหาการตั้งค่า DKIM

ถ้าคุณพบปัญหาในการเปิดใช้งาน DKIM ของโดเมนแบบปรับแต่งเองของคุณ ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

- ปัญหาการตั้งค่า DKIM ส่วนใหญ่เกี่ยวข้องกับระเบียน DNS ที่ไม่ถูกต้อง ตรวจสอบระเบียน CNAME ของ DKIM **(ไม่ใช่** ระเบียน TXT) ถูกจัดรูปแบบอย่างถูกต้อง หากต้องการข้อมูลเพิ่มเติม [โปรดดู](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)หัวข้อนี้

- หลังจากที่คุณสร้างหรืออัปเดตระเบียน DNS DKIM ของคุณที่บริการการโฮสต์ DNS ของโดเมนของคุณ (โดยทั่วไปคือ บริษัทจดทะเบียนโดเมนของคุณ) ให้รอให้ระเบียน DNS เผยแพร่

- ถ้าคุณไม่สามารถสร้างระเบียน DNS DKIM ในศูนย์การจัดการ คุณสามารถแทนที่ด้วยโดเมนแบบปรับแต่งเองของคุณ (ตัวอย่างเช่น contoso.com) และเรียกใช้สั่งนี้Exchange Online \<CustomDomain\> [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`
