---
title: อัปเดตเนมเซิร์ฟเวอร์ของโดเมนให้ชี้ไปยัง Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: d9d66e366db14840a86b681deba78b89ddff5e068a3b931c88e493d2ec791b10
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54073619"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>อัปเดตเนมเซิร์ฟเวอร์ของโดเมนให้ชี้ไปยัง Microsoft

หมายเหตุ: บางครั้งการเปลี่ยนแปลงเซิร์ฟเวอร์ชื่ออาจใช้เวลาถึง 48 ชั่วโมงในการเผยแพร่
  
เมื่อต้องการตั้งค่าโดเมนของคุณด้วย Microsoft จะต้องอัปเดตเนมเซิร์ฟเวอร์ที่บริษัทจดทะเบียนของคุณ สร้างหรือแก้ไขระเบียนเนมเซิร์ฟเวอร์ของคุณที่บริษัทจดทะเบียนโดเมนของคุณ
  
1. ไปที่เว็บไซต์ของบริษัทจดทะเบียนโดเมนของคุณ และค้นหาพื้นที่ที่คุณสามารถแก้ไขเนมเซิร์ฟเวอร์ได้

2. สร้างหรือแก้ไขระเบียนเนมเซิร์ฟเวอร์สองระเบียนให้ตรงกับค่าเหล่านี้:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. บันทึกการเปลี่ยนแปลง

คุณยังสามารถค้นหาคําแนะนําโดยละเอียดในบทความนี้:[เปลี่ยนเนมเซิร์ฟเวอร์เพื่อตั้งค่าMicrosoft 365กับบริษัทจดทะเบียนโดเมน](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  