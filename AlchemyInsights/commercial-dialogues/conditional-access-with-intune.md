---
title: การใช้การเข้าถึงตามเงื่อนไขด้วย Intun1
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
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749265"
---
# <a name="using-conditional-access-with-intune"></a>การใช้การเข้าถึงตามเงื่อนไขด้วย Intun1

การใช้การเข้าถึงตามเงื่อนไขด้วย Intun1 ต้องมี 3 ขั้นตอน:

- [สร้างนโยบายการปฏิบัติตามนโยบายเพื่อกําหนดการตั้งค่าที่ต้องปฏิบัติตามก่อนที่จะถือว่าอุปกรณ์ปฏิบัติตามนโยบายแล้ว ตัวอย่างเช่น อุปกรณ์ต้องมีรหัส PIN อย่างน้อย 6 หลักก่อนที่จะถือว่าตรงตามมาตรฐาน](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [สร้างนโยบายการเข้าถึงตามเงื่อนไขที่กําหนดว่าทรัพยากรใดที่ได้รับการป้องกัน และเงื่อนไขที่ต้องใช้เพื่อเข้าถึงทรัพยากรเหล่านั้น ตัวอย่างเช่น อุปกรณ์จะต้องปฏิบัติตามนโยบายก่อนที่จะเข้าถึงอีเมลของบริษัท](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [ตรวจสอบให้แน่ใจว่านโยบายการปฏิบัติตามนโยบายและนโยบายการเข้าถึงตามเงื่อนไขถูกตั้งเป้าหมายไปยังกลุ่มผู้ใช้ที่ต้องการ ซึ่งอาจต้องมีการสร้างกลุ่มเฉพาะของผู้ใช้ใน Azure Active Directory](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[อ่านเพิ่มเติม...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
