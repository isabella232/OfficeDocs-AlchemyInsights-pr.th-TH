---
title: แก้ไขปัญหาการติดตั้ง DKIM
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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717581"
---
# <a name="fix-dkim-setup-issues"></a>แก้ไขปัญหาการติดตั้ง DKIM

หากคุณประสบปัญหาในการเปิดใช้ DKIM สําหรับโดเมนแบบกําหนดเอง ให้ทําตามขั้นตอนต่อไปนี้

- ปัญหาการตั้งค่า DKIM ส่วนใหญ่เกี่ยวข้องกับระเบียน DNS ที่ไม่ถูกต้อง ตรวจสอบว่าระเบียน CNAME DKIM (**ไม่ใช่**ระเบียน TXT) ถูกจัดรูปแบบอย่างถูกต้อง สําหรับข้อมูลเพิ่มเติม ให้ดูที่[หัวข้อนี้](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)

- หลังจากที่คุณสร้างหรืออัปเดตระเบียน DNS DKIM ที่บริการโฮสต์ DNS สําหรับโดเมนของคุณ (โดยทั่วไปแล้ว

- ถ้าคุณไม่สามารถสร้างระเบียน DNS DKIM ใน\<contoso.com\>[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)`New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`ศูนย์การจัดการ
