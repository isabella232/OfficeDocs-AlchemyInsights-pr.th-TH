---
title: การเข้าถึงตามเงื่อนไขด้วย Intun1
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069731"
---
# <a name="conditional-access-with-intune"></a>การเข้าถึงตามเงื่อนไขด้วย Intun1

การใช้  **การเข้าถึงตามเงื่อนไขกับ**  Intun1 ต้องมี 3 ขั้นตอน:

- สร้างนโยบาย **การปฏิบัติตามนโยบาย**([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) เพื่อกําหนดการตั้งค่าที่ต้องปฏิบัติตามก่อนที่จะถือว่าอุปกรณ์ปฏิบัติตามนโยบายแล้ว ตัวอย่างเช่น อุปกรณ์ต้องมีรหัส PIN อย่างน้อย 6 หลักก่อนที่จะถือว่าสอดคล้อง
- สร้าง **นโยบายการเข้าถึงตามเงื่อนไข**  ที่กําหนดว่าทรัพยากรใดที่ได้รับการป้องกัน และเงื่อนไขที่คุณต้องเป็นไปตามเพื่อเข้าถึงทรัพยากรเหล่านั้น  [ตัวอย่างเช่น จะต้อง](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  ปฏิบัติตามนโยบายอุปกรณ์ก่อนที่จะเข้าถึงอีเมลของบริษัท
- ตรวจสอบให้แน่ใจว่า **ได้ตั้ง****เป้าหมายนโยบายการปฏิบัติตามนโยบาย** และนโยบายการเข้าถึงตามเงื่อนไขไปยังกลุ่มผู้ใช้ที่ต้องการแล้ว ซึ่งอาจต้องมีการสร้างกลุ่มของผู้ใช้ที่เฉพาะเจาะจงในAzure Active Directoryของคุณ

**ลิงก์ที่มีประโยชน์:**

[ภาพรวมการปฏิบัติตามนโยบายอุปกรณ์](https://docs.microsoft.com/intune/device-compliance-get-started)

[การแก้ไขปัญหา CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[การแก้ไขปัญหานโยบาย](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

เพื่อป้องกันอีเมล (Exchangeออนไลน์) จากการเข้าถึงด้วยอุปกรณ์ที่ไม่เข้ากัน ต้องปฏิบัติตามเอกสารทั้งสองอย่างดังนี้

1. [ป้องกันการเข้าถึงอีเมลจากอุปกรณ์โดยใช้ EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [ป้องกันการเข้าถึงอีเมลจากอุปกรณ์โดยใช้ไคลเอ็นต์การรับรองความถูกต้องOutlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)