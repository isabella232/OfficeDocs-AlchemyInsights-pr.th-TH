---
title: การใช้เว็บไซต์ Wix กับ Office 365 ที่ซื้อหรือโดเมนที่มีการจัดการ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825966"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>การใช้เว็บไซต์ Wix กับ Office 365 ที่ซื้อหรือโดเมนที่มีการจัดการ

- [อัปเดตระเบียน DNS เพื่อเก็บเว็บไซต์ของคุณกับผู้ให้บริการโฮสต์ปัจจุบันของคุณ](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- บทความ Wix "การเชื่อมต่อโดเมนกับ Wix โดยใช้วิธีการชี้" ขอแนะนการใช้การชี้ (การเพิ่มระเบียน DNS ต่อลิงก์ด้านบน) แทนการเปลี่ยนเซิร์ฟเวอร์ชื่อเมื่อใช้ Office 365
- If you still choose to change name servers to Wix you will then need to  [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- ถ้าโดเมนของคุณถูกซื้อจาก Microsoft เซิร์ฟเวอร์ชื่อจะไม่สามารถเปลี่ยนแปลงได้ ถ้าคุณต้องเปลี่ยนเซิร์ฟเวอร์ชื่อ โดเมนที่ซื้อโดย Microsoft จะต้องถูกถ่ายโอน  [ไปยังผู้ให้บริการโฮสต์อื่นหลังจาก 60 วัน](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)