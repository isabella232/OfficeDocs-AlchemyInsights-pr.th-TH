---
title: อัปเดเซิร์ฟเวอร์ชื่อโดเมนของคุณให้ชี้ไปที่ Microsoft
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
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734930"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>อัปเดเซิร์ฟเวอร์ชื่อโดเมนของคุณให้ชี้ไปที่ Microsoft

หมายเหตุ: การเปลี่ยนแปลง Nameserver บางครั้งอาจใช้เวลาถึง๔๘ชั่วโมงในการเผยแพร่
  
เมื่อต้องการตั้งค่าโดเมนของคุณด้วย Microsoft การเซิร์ฟเวอร์ชื่อที่บริษัทจดทะเบียนของคุณจำเป็นต้องได้รับการอัปเดต สร้างหรือแก้ไขระเบียน nameserver ของคุณที่บริษัทจดทะเบียนโดเมนของคุณ
  
1. ไปที่เว็บไซต์ของบริษัทจดทะเบียนโดเมนของคุณและค้นหาพื้นที่ที่คุณสามารถแก้ไขเซิร์ฟเวอร์ชื่อได้

2. สร้างหรือแก้ไขระเบียน nameserver สองระเบียนให้ตรงกับค่าเหล่านี้:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. บันทึกการเปลี่ยนแปลง

นอกจากนี้คุณยังสามารถค้นหาคำแนะนำโดยละเอียดในบทความนี้:[เปลี่ยนเซิร์ฟเวอร์ชื่อเพื่อตั้งค่า Microsoft ๓๖๕กับบริษัทจดทะเบียนโดเมนใดก็](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)ได้
  