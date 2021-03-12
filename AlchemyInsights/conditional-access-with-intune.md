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
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704805"
---
# <a name="conditional-access-with-intune"></a>การเข้าถึงตามเงื่อนไขด้วย Intun1

การใช้  **การเข้าถึงตามเงื่อนไขด้วย**  Intun1 ต้องมี 3 ขั้นตอน:

- สร้างนโยบาย  **การปฏิบัติตามนโยบาย**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) เพื่อกําหนดการตั้งค่าที่ต้องปฏิบัติตามก่อนที่จะถือว่าอุปกรณ์ปฏิบัติตามนโยบายแล้ว ตัวอย่างเช่น อุปกรณ์ต้องมีรหัส PIN อย่างน้อย 6 หลักก่อนที่จะถือว่าตรงตามมาตรฐาน
- สร้าง **นโยบายการเข้าถึงตามเงื่อนไข**  ที่กําหนดว่าทรัพยากรใดที่ได้รับการป้องกัน และเงื่อนไขที่ต้องใช้เพื่อเข้าถึงทรัพยากรเหล่านั้น  [ตัวอย่างเช่น อุปกรณ์](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  จะต้องปฏิบัติตามนโยบายก่อนที่จะเข้าถึงอีเมลของบริษัท
- ตรวจสอบให้แน่ใจ **ว่านโยบายการปฏิบัติตาม****นโยบายและนโยบายการเข้าถึง** ตามเงื่อนไขถูกตั้งเป้าหมายไปยังกลุ่มผู้ใช้ที่ต้องการ ซึ่งอาจต้องมีการสร้างกลุ่มเฉพาะของผู้ใช้ใน Azure Active Directory

**ลิงก์ที่เป็นประโยชน์:**

[ภาพรวมการปฏิบัติตามนโยบายอุปกรณ์](https://docs.microsoft.com/intune/device-compliance-get-started)

[การแก้ไขปัญหา CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[การแก้ไขปัญหานโยบาย](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

เมื่อต้องการป้องกันอีเมล (Exchange Online) จากการเข้าถึงด้วยอุปกรณ์ที่ไม่เข้ากัน ต้องปฏิบัติตามทั้งสองเอกสาร:

1. [ป้องกันการเข้าถึงอีเมลจากอุปกรณ์โดยใช้ EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [ป้องกันการเข้าถึงอีเมลจากอุปกรณ์โดยใช้ไคลเอ็นต์การรับรองความถูกต้องสมัยใหม่ เช่น Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)