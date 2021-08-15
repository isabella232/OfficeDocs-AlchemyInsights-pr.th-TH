---
title: ตั้งค่า DKIM ด้วยโดเมนแบบปรับแต่งเอง
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: bb19f0672a21ea8b99c433ad83db4d89536c9a1705245fd2a683471170ab51ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994848"
---
# <a name="set-up-dkim-with-custom-domains"></a>ตั้งค่า DKIM ด้วยโดเมนแบบปรับแต่งเอง

คุณต้องเผยแพร่ระเบียน CNAME สองระเบียนในแต่ละโดเมนแบบปรับแต่งเองใน DNS เมื่อต้องการใช้วิธีนี้ ให้ใช้รูปแบบต่อไปนี้:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** คือข้อความที่อยู่ทางด้านซ้ายของ **.mail.protection.outlook.com** ในระเบียน MX ที่ปรับแต่งเองของโดเมนแบบปรับแต่งเอง (ตัวอย่างเช่น contoso-com contoso.com ) **InitialDomain** คือโดเมนที่คุณใช้เมื่อคุณลงทะเบียนOffice 365โดเมนของคุณ (ตัวอย่างเช่น **contoso.onmicrosoft.com)**

For more information about DNS records, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).