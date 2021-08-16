---
title: 2681 Attack In Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: b173c6eb3bbbd1beba3b59878ae12bbe7684d0447a16fef746e5b97b82349e53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065303"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack In Microsoft 365

- คุณพลาด Attack 11 ใช่หรือไม่ Attack Defender ต้องใช้ **Microsoft Defender Office 365 Plan 2** หรือ Office 365 Enterprise **E5** Attack Defender **จะไม่** รวมอยู่ใน Microsoft Defender Office 365 Plan 1, Office 365 Enterprise E3 หรือMicrosoft 365 Apps for businessอื่น ๆ

- บัญชีที่คุณใช้เพื่อเปิดใช้การโจมตีที่จําเป็นต้องมีผู้ดูแลระบบส่วนกลางหรือสิทธิ์ของผู้ดูแลระบบความปลอดภัยและการรับรองความถูกต้องโดยใช้หลายปัจจัย (MFA) For more information about Attack Attack Attack requirements, [see this](/microsoft-365/security/office-365-security/attack-simulator)topic .

- สิ่งสําคัญที่ควรทราบ **เกี่ยวกับสถานการณ์โจมตีของ Brute Force** Password:

  - ถ้าบัญชีเป้าหมายเปิดใช้งาน MFA และรหัสผ่านคาดเดาไม่ถูกต้อง บัญชีจะไม่แสดงเป็นบัญชีที่ถูกละเมิด (ปัจจัยการรับรองความถูกต้องที่สองจะไม่สมบูรณ์)

  - ไฟล์รหัสผ่านไม่สามารถมีขนาดใหญ่กว่า 10 MB ได้ ใช้รหัสผ่านหนึ่งรหัสผ่านต่อบรรทัด และใส่บรรทัดว่าง (อักขระขึ้นบรรทัดใหม่) หลังรหัสผ่านสุดท้ายในรายการ

- สิ่งสําคัญที่ควรทราบ **เกี่ยวกับฟิชชิ่งของ Phishing** แนบการสถานการณ์:

  - ตามการออกแบบ คุณไม่สามารถใส่ URL ของเซิร์ฟเวอร์การเข้าสู่ระบบฟิชชิ่ง

  - ถ้าผู้รับใช้ [Add-in เปิดใช้งานข้อความ](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) รายงาน เพื่อรายงานข้อความเป็นฟิชชิ่ง คุณอาจไม่ได้รับการแจ้งเตือนข้อความนั้น (เนื่องจากนี่คือการโจมตีที่จําเป็น)

- รายงาน: หลังจากการโจมตีที่จําเป็นเสร็จสมบูรณ์ คุณสามารถ **คลิก รายละเอียด** การโจมตี เพื่อดูรายงานได้

- ดูคําแนะนําโดยละเอียดและฟีเจอร์ใหม่ใน Attackขออภัย[ให้ดู Attackขออภัยใน Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator)
