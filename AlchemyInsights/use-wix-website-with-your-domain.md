---
title: การใช้เว็บไซต์ Wix กับโดเมนที่ซื้อหรือจัดการของ Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 64dfe6082bea1e468eae78bf1576fde398e4c28a
ms.sourcegitcommit: 3ca312535d950105ee829e037f0ff8f1ddbbae72
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/11/2020
ms.locfileid: "44708503"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>การใช้เว็บไซต์ Wix กับโดเมนที่ซื้อหรือจัดการของ Office 365

- [อัปเดตระเบียน DNS เพื่อเก็บเว็บไซต์ของคุณกับผู้ให้บริการโฮสต์ปัจจุบันของคุณ](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- บทความ Wix "การเชื่อมต่อโดเมนกับ Wix โดยใช้วิธีการชี้ตําแหน่ง" แนะนําการใช้ชี้ (เพิ่มระเบียน DNS ต่อการเชื่อมโยงด้านบน) แทนที่จะเปลี่ยนชื่อเซิร์ฟเวอร์เมื่อใช้ Office 365
- หากคุณยังคงเลือกที่จะเปลี่ยนเซิร์ฟเวอร์ชื่อเป็น Wix คุณจะต้อง[สร้างระเบียน DNS ที่ Wix สําหรับ Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- ถ้าโดเมนของคุณซื้อจาก Microsoft เซิร์ฟเวอร์ชื่อไม่สามารถเปลี่ยนแปลงได้ ถ้าคุณต้องเปลี่ยนชื่อเซิร์ฟเวอร์โดเมนที่ซื้อของ Microsoft จะต้อง[ถูกถ่ายโอนไปยังผู้ให้บริการโฮสต์อื่นหลังจาก 60 วัน](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)