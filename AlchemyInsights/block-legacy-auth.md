---
title: บล็อกดั้งเดิม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: e7bff5f9fcf6f2f2c77e93c2f27f585f2cc18bea
ms.sourcegitcommit: 98231a228ecb2bf14ec3b96d4dd4ccf2507617a3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/01/2020
ms.locfileid: "43079279"
---
# <a name="blocking-legacy-authentication"></a>การบล็อกการรับรองความถูกต้องแบบดั้งเดิม

การรับรองความถูกต้องแบบดั้งเดิมเป็นคําที่อ้างถึงการร้องขอการรับรองความถูกต้องที่ทําโดย:

- ไคลเอ็นต์ Office เก่าที่ไม่ได้ใช้การรับรองความถูกต้องแบบสมัยใหม่ (ตัวอย่างเช่น ไคลเอ็นต์ Office 2010)

- ไคลเอ็นต์ใด ๆ ที่ใช้โพรโทคอลจดหมายแบบดั้งเดิมเช่น IMAP/SMTP/POP3

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการบล็อกการรับรองความถูกต้องแบบดั้งเดิมและเปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่ ให้ดูที่[การบล็อกการรับรองความถูกต้องแบบดั้งเดิม](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)

ค่าเริ่มต้นการรักษาความปลอดภัยใน Azure Active Directory (Azure AD) ช่วยให้มีความปลอดภัยและช่วยปกป้ององค์กรของคุณได้ง่ายขึ้น ค่าเริ่มต้นความปลอดภัยมีการตั้งค่าความปลอดภัยที่กําหนดไว้ล่วงหน้าสําหรับการโจมตีทั่วไป
สําหรับข้อมูลเพิ่มเติมเกี่ยวกับค่าเริ่มต้นความปลอดภัย ให้ดูที่[ค่าเริ่มต้นความปลอดภัยคืออะไร](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) 

**หมายเหตุ**: ถ้าผู้เช่าของคุณถูกสร้างขึ้นในวันที่ หรือหลังวันที่ 22 ตุลาคม 2019 เป็นไปได้ว่าคุณประสบกับลักษณะการทํางานที่ปลอดภัยโดยเริ่มต้นใหม่ และได้เปิดใช้ค่าเริ่มต้นการรักษาความปลอดภัยในผู้เช่าของคุณแล้ว  ในความพยายามที่จะปกป้องผู้ใช้ทั้งหมดของเราค่าเริ่มต้นการรักษาความปลอดภัยจะถูกรีดออกไปยังผู้เช่าใหม่ทั้งหมดที่สร้างขึ้น
