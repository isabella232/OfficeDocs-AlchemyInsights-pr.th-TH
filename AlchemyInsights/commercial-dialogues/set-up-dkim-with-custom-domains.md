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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332326"
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
**หมายเหตุ**: **DomainGUID** คือข้อความทางด้านซ้ายของ **.mail.protection.outlook.com** ในระเบียน MX ที่ปรับแต่งเองของโดเมนแบบปรับแต่งเอง (ตัวอย่างเช่น contoso-com for the domain **contoso.com)** **InitialDomain** คือโดเมนที่คุณใช้เมื่อคุณลงทะเบียนOffice 365โดเมนของคุณ **(contoso.onmicrosoft.com)**

For more information about DNS records, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).