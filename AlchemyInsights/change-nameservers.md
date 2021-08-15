---
title: เปลี่ยนเซิร์ฟเวอร์ชื่อ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 3f39bfc585e8b805424cb7ccac76f81e1b2bfda9dcd1367361fec6a668c545bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017799"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>อัปเดตเนมเซิร์ฟเวอร์ของโดเมนให้ชี้ไปยัง Microsoft

หมายเหตุ: บางครั้งการเปลี่ยนแปลงเซิร์ฟเวอร์ชื่ออาจใช้เวลาถึง 48 ชั่วโมงในการเผยแพร่
  
เมื่อต้องการตั้งค่าโดเมนMicrosoft 365 เซิร์ฟเวอร์ชื่อที่บริษัทจดทะเบียนของคุณต้องได้รับการอัปเดต สร้างหรือแก้ไขระเบียนเนมเซิร์ฟเวอร์ของคุณที่บริษัทจดทะเบียนโดเมนของคุณ
  
1. ไปที่เว็บไซต์ของบริษัทจดทะเบียนโดเมนของคุณ และค้นหาพื้นที่ที่คุณสามารถแก้ไขเนมเซิร์ฟเวอร์ได้
  
2. สร้างหรือแก้ไขระเบียนเนมเซิร์ฟเวอร์สองระเบียนให้ตรงกับค่าเหล่านี้:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. บันทึกการเปลี่ยนแปลง

คุณยังสามารถค้นหาคําแนะนําโดยละเอียดในบทความนี้: [เปลี่ยนเนมเซิร์ฟเวอร์กับบริษัทจดทะเบียนโดเมน](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  