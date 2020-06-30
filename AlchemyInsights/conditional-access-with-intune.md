---
title: การเข้าถึงแบบมีเงื่อนไขกับ Intun
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931455"
---
# <a name="conditional-access-with-intune"></a>การเข้าถึงแบบมีเงื่อนไขกับ Intun

การใช้**การเข้าถึงแบบมีเงื่อนไข**กับ Intunเน จําเป็นต้องมีขั้นตอนที่ 3:

- สร้าง**นโยบายการปฏิบัติตามกฎระเบียบ**([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) เพื่อกําหนดการตั้งค่าที่ต้องเป็นไปตามก่อนที่อุปกรณ์จะถือว่าเป็นไปตาม ตัวอย่างเช่น อุปกรณ์ต้องมีหมุดอย่างน้อย 6 หลักก่อนที่จะถือว่าเป็นไปตามข้อกําหนด
- สร้าง**นโยบายการเข้าถึงแบบมีเงื่อนไข**ที่กําหนดทรัพยากรที่ถูกป้องกัน และต้องเป็นไปตามเงื่อนไขใดเพื่อเข้าถึงทรัพยากรเหล่านั้น  [ตัวอย่างเช่น](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)อุปกรณ์ต้องเป็นไปตามข้อกําหนดก่อนที่จะเข้าถึงอีเมลขององค์กร
- ตรวจสอบให้แน่ใจว่านโยบาย**การปฏิบัติตามกฎระเบียบ**และ**นโยบายการเข้าถึงตามเงื่อนไข**ถูกกําหนดเป้าหมายไปยังกลุ่มผู้ใช้ที่ต้องการ ซึ่งอาจต้องใช้การสร้างกลุ่มเฉพาะของผู้ใช้ในไดเรกทอรีที่ใช้งานอยู่ของ Azure

**การเชื่อมโยงที่เป็นประโยชน์:**

[ภาพรวมการปฏิบัติตามข้อกําหนดของอุปกรณ์](https://docs.microsoft.com/intune/device-compliance-get-started)

[การแก้ไขปัญหา CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[นโยบายการแก้ไขปัญหา](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

เมื่อต้องการป้องกันอีเมล (Exchange แบบออนไลน์) จากการเข้าถึง โดยอุปกรณ์ที่ไม่ปฏิบัติตาม เอกสารทั้งสองต้องปฏิบัติตาม:

1. [ปกป้องการเข้าถึงอีเมลจากอุปกรณ์โดยใช้ EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [ป้องกันการเข้าถึงอีเมลจากอุปกรณ์โดยใช้ไคลเอ็นต์การรับรองความถูกต้องแบบสมัยใหม่เช่น Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)