---
title: แก้ไขปัญหาการตั้งค่า DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506793"
---
# <a name="fix-dkim-setup-issues"></a>แก้ไขปัญหาการตั้งค่า DKIM

หากคุณพบปัญหาในการเปิดใช้งาน DKIM สําหรับโดเมนแบบกําหนดเอง ของคุณ ให้ใช้ขั้นตอนต่อไปนี้

- ปัญหาการตั้งค่า DKIM ส่วนใหญ่เกี่ยวข้องกับระเบียน DNS ที่ไม่ถูกต้อง ตรวจสอบระเบียน CNAME DKIM (**ไม่ใช่**ระเบียน TXT) ถูกจัดรูปแบบอย่างถูกต้อง สําหรับข้อมูลเพิ่มเติม ให้ดูที่[หัวข้อนี้](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- หลังจากที่คุณสร้างหรืออัปเดตระเบียน DNS DKIM ของคุณที่บริการโฮสต์ DNS สําหรับโดเมนของคุณ (โดยทั่วไปแล้ว

- ถ้าคุณไม่สามารถสร้างระเบียน DNS DKIM ใน \<CustomDomain\> contoso.com[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)ศูนย์การจัดการ `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`
