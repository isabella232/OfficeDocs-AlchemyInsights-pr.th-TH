---
title: การเข้าถึงตามเงื่อนไขด้วย Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807678"
---
# <a name="conditional-access-with-intune"></a>การเข้าถึงตามเงื่อนไขด้วย Intune

การใช้การ  **เข้าถึง**  แบบมีเงื่อนไขด้วย Intune จำเป็นต้องมี3ขั้นตอนดังนี้

- สร้าง  **นโยบายการปฏิบัติตามนโยบาย**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) เพื่อกำหนดการตั้งค่าที่ต้องเป็นไปตามก่อนที่อุปกรณ์จะถือว่าเป็นไปตามนโยบาย ตัวอย่างเช่นอุปกรณ์จำเป็นต้องมี pin อย่างน้อย6หลักก่อนที่จะถือว่าสอดคล้องกัน
- สร้าง **นโยบายการเข้าถึงตามเงื่อนไข**  ที่กำหนดว่าทรัพยากรใดบ้างที่ได้รับการป้องกันและต้องเป็นไปตามเงื่อนไขใดในการเข้าถึงแหล่งข้อมูลเหล่านั้น  ตัว[อย่างเช่น](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)อุปกรณ์ต้องสอดคล้องก่อนที่จะเข้าถึงอีเมลขององค์กร
- ตรวจสอบให้แน่ใจ **ว่านโยบายการปฏิบัติตามกฎระเบียบ**  และ  **นโยบายการเข้าถึงตามเงื่อนไข**  จะถูกกำหนดเป้าหมายให้กับกลุ่มผู้ใช้ที่ต้องการ การทำเช่นนี้อาจจำเป็นต้องสร้างกลุ่มผู้ใช้ที่เฉพาะเจาะจงใน Azure Active Directory

**ลิงก์ที่มีประโยชน์:**

[ภาพรวมการปฏิบัติตามกฎระเบียบของอุปกรณ์](https://docs.microsoft.com/intune/device-compliance-get-started)

[การแก้ไขปัญหา CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[นโยบายการแก้ไขปัญหา](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

เมื่อต้องการป้องกันอีเมล (Exchange online) จาก access โดยอุปกรณ์ noncompliant เอกสารทั้งสองต้องเป็นไปตาม:

1. [ป้องกันการเข้าถึงอีเมลจากอุปกรณ์ที่ใช้ EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [ป้องกันการเข้าถึงอีเมลจากอุปกรณ์ที่ใช้ไคลเอ็นต์การรับรองความถูกต้องที่ทันสมัยเช่น Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)