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
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525422"
---
# <a name="set-up-dkim-with-custom-domains"></a>ตั้งค่า DKIM ด้วยโดเมนแบบปรับแต่งเอง

คุณต้องเผยแพร่ระเบียน CNAME สองระเบียนในแต่ละโดเมนแบบปรับแต่งเองใน DNS เมื่อต้องการใช้รูปแบบต่อไปนี้:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** คือข้อความทางซ้ายของ **.mail.protection.outlook.com** ในระเบียน MX แบบปรับแต่งเองของโดเมนแบบเอง (ตัวอย่างเช่น contoso-com for the domain **contoso.com)** **InitialDomain** คือโดเมนที่คุณใช้เมื่อคุณลงทะเบียน Office 365 (ตัวอย่างเช่น **contoso.onmicrosoft.com)**

For more information about DNS records, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).