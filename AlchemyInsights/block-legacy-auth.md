---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: c2f2a0c3888920a969a6fc70af7ef7bfd8435bdcf975e0f31452b5da85e3a208
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968900"
---
# <a name="blocking-legacy-authentication"></a>การบล็อกการรับรองความถูกต้องแบบดั้งเดิม

การรับรองความถูกต้องแบบดั้งเดิมคือศัพท์ที่อ้างอิงถึงการร้องขอการรับรองความถูกต้องที่ถูกสร้างขึ้นโดย:

- ไคลเอ็นต์Officeเก่าที่ไม่ได้ใช้การรับรองความถูกต้องแบบใหม่ (ตัวอย่างเช่น Office 2010)

- ไคลเอ็นต์ใดๆ ที่ใช้โพรโทคอลจดหมายแบบดั้งเดิม เช่น IMAP/SMTP/POP3

For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).

ค่าเริ่มต้นด้านความปลอดภัยAzure Active Directory (Azure AD) ช่วยให้คุณปลอดภัยและช่วยปกป้ององค์กรของคุณได้ง่ายขึ้น ค่าเริ่มต้นด้านความปลอดภัยประกอบด้วยการตั้งค่าความปลอดภัยที่ตั้งค่าไว้ล่วงหน้าของการโจมตีทั่วไป
For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults). 

**หมายเหตุ**: ถ้าผู้เช่าของคุณถูกสร้างขึ้นในวันที่ 22 ตุลาคม 2019 หรือหลังจากวันที่ 22 ตุลาคม 2019 อาจเป็นไปได้ว่าคุณประสบกับลักษณะการรักษาความปลอดภัยตามค่าเริ่มต้นแบบใหม่ และมีการเปิดใช้งานค่าเริ่มต้นด้านความปลอดภัยในผู้เช่าของคุณอยู่แล้ว  ในความพยายามในการปกป้องผู้ใช้ของเราทั้งหมด ค่าเริ่มต้นด้านความปลอดภัยจะทยให้ผู้เช่าใหม่ทั้งหมดถูกสร้างขึ้น
