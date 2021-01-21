---
title: กำหนดค่าและขยายระยะเวลาของโทเค็น
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
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917197"
---
# <a name="configure-and-extend-token-lifetimes"></a>กำหนดค่าและขยายระยะเวลาของโทเค็น

คุณสามารถระบุอายุการใช้งานของโทเค็นการเข้าถึง SAML หรือ ID ที่ออกโดย Microsoft identity platform คุณสามารถตั้งค่าการหมดอายุของโทเค็นสำหรับแอปทั้งหมดในองค์กรของคุณสำหรับแอปพลิเคชันแบบหลายผู้เช่า (หลายองค์กร) หรือสำหรับบริการหลักที่เฉพาะเจาะจงในองค์กรของคุณ สำหรับข้อมูลเพิ่มเติมให้อ่านช่วงเวลาของ [โทเค็น](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)ที่กำหนดค่าไว้

ตัวอย่างเช่นอ่าน[ตัวอย่างของวิธีการกำหนดค่าการหมดอายุของโทเค็น](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)

เมื่อต้องการเรียนรู้วิธีการกำหนดค่าอายุการใช้งานและความเข้ากันได้ของโทเค็นใน Azure Active Directory B2C (Azure AD B2C) ให้ดู [ที่การกำหนดค่าโทเค็นใน B2C Azure active](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)directory

บทความการ [กำหนดค่าลักษณะการทำงานของเซสชันใน B2C Azure active](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) directory จะอธิบายวิธีการลงชื่อเข้าระบบครั้งเดียว (SSO) ที่ใช้ใน B2C AD Azure และช่วยให้คุณเลือกวิธีที่เหมาะสมที่สุดของ SSO เมื่อกำหนดค่านโยบายของคุณ

**โทเค็นจะมีระยะเวลานานแค่ไหน พวกเขาจะใช้งานได้นานแค่ไหน**

อายุการใช้งานของโทเค็นคือ1ชั่วโมงและอายุการใช้งานของเซสชันคือ24ชั่วโมง ซึ่งหมายความว่าถ้าไม่มีการร้องขอใน24ชั่วโมงคุณจำเป็นต้องเข้าสู่ระบบอีกครั้งก่อนที่จะร้องขอโทเค็นใหม่

> [!NOTE]
> หลังจาก30พฤษภาคม๒๐๒๐ไม่มีผู้เช่าใหม่จะสามารถใช้นโยบายอายุการใช้งานโทเค็นที่กำหนดค่าเพื่อกำหนดค่าเซสชันและการรีเฟรชโทเค็น แผนจะเกิดขึ้นภายในหลายเดือนหลังจากนั้นซึ่งหมายความว่าเราจะหยุดการ honoring เซสชันที่มีอยู่และการรีเฟรช คุณยังสามารถกำหนดค่าความหมดอายุของโทเค็นการเข้าถึงหลังจากแผนได้






