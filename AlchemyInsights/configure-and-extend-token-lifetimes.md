---
title: กําหนดค่าและขยายอายุการใช้งานโทเค็น
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: ce100fcc2c62d62477f78e10b3cc9233fc2f5c5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329105"
---
# <a name="configure-and-extend-token-lifetimes"></a>กําหนดค่าและขยายอายุการใช้งานโทเค็น

คุณสามารถระบุอายุการใช้งานของการเข้าถึง, โทเค็น SAML หรือ ID ที่ออกโดยแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft คุณสามารถตั้งค่าอายุการใช้งานโทเค็นของแอปทั้งหมดในองค์กรของคุณ, แอปพลิเคชันแบบหลายผู้เช่า (หลายองค์กร) หรือแอปพลิเคชันหลักบริการเฉพาะในองค์กรของคุณได้ For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

ตัวอย่างเช่น อ่าน [ตัวอย่างของวิธีการกําหนดค่าอายุการใช้งาน](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)โทเค็น

เมื่อต้องการเรียนรู้วิธีการกําหนดค่าอายุการใช้งานและความเข้ากันได้ของโทเค็นใน Azure Active Directory B2C (Azure AD B2C) ให้ดู กําหนดค่าโทเค็น[ใน Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)

บทความ การกําหนดค่าลักษณะการใช้งานได้ของเซสชันใน [Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) จะอธิบายวิธีการลงชื่อเข้าระบบครั้งเดียว (SSO) ที่ใช้ใน Azure AD B2C และช่วยให้คุณเลือกวิธีการ SSO ที่เหมาะสมที่สุดเมื่อกําหนดค่านโยบายของคุณ

**โทเค็นจะอยู่นานเท่าใด ระยะเวลาที่ใช้ได้**

อายุการใช้งานโทเค็นคือ 1 ชั่วโมง และอายุการใช้งานเซสชันคือ 24 ชั่วโมง ซึ่งหมายความว่าถ้าไม่มีการร้องขอใดเกิดขึ้นภายใน 24 ชั่วโมง คุณจะต้องเข้าสู่ระบบอีกครั้งก่อนที่จะร้องขอโทเค็นใหม่

**หมายเหตุ**: หลังจากวันที่ 30 พฤษภาคม 2020 ไม่มีผู้เช่าใหม่ที่สามารถใช้นโยบายอายุการใช้งานโทเค็นที่กําหนดค่าได้เพื่อกําหนดค่าโทเค็นเซสชันและรีเฟรช การเลิกใช้จะเกิดขึ้นภายในเวลาหลายเดือนหลังจากนั้น ซึ่งหมายความว่าเราจะหยุดเคารพเซสชันที่มีอยู่และรีเฟรชโทเค็นตวจ คุณยังสามารถกําหนดค่าอายุการใช้งานโทเค็นการเข้าถึงได้หลังจากการเลิกใช้






