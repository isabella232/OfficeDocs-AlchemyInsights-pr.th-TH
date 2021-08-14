---
title: การใช้การเข้าถึงตามเงื่อนไขกับ Intun1
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005793"
---
# <a name="using-conditional-access-with-intune"></a>การใช้การเข้าถึงตามเงื่อนไขกับ Intun1

การใช้ การเข้าถึงตามเงื่อนไขกับ Intun1 ต้องมี 3 ขั้นตอน:

- [สร้างนโยบายการปฏิบัติตามนโยบายเพื่อกําหนดการตั้งค่าที่ต้องปฏิบัติตามก่อนที่จะถือว่าอุปกรณ์ปฏิบัติตามนโยบายแล้ว ตัวอย่างเช่น อุปกรณ์ต้องมีรหัส PIN อย่างน้อย 6 หลักก่อนที่จะถือว่าสอดคล้อง](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [สร้างนโยบายการเข้าถึงตามเงื่อนไขที่กําหนดว่าทรัพยากรใดที่ได้รับการป้องกัน และเงื่อนไขที่คุณต้องเป็นไปตามเพื่อเข้าถึงทรัพยากรเหล่านั้น ตัวอย่างเช่น จะต้องปฏิบัติตามนโยบายอุปกรณ์ก่อนที่จะเข้าถึงอีเมลของบริษัท](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [ตรวจสอบให้แน่ใจว่าได้ตั้งเป้าหมายนโยบายการปฏิบัติตามนโยบายและนโยบายการเข้าถึงตามเงื่อนไขไปยังกลุ่มผู้ใช้ที่ต้องการแล้ว ซึ่งอาจต้องมีการสร้างกลุ่มของผู้ใช้ที่เฉพาะเจาะจงในAzure Active Directoryของคุณ](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[อ่านเพิ่มเติม...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
