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
ms.openlocfilehash: f6e221cc82a1b707f6acc457cb78db743521d859
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325090"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack In Microsoft 365

- คุณพลาด Attack 11 ใช่หรือไม่ Attack Defender ต้องใช้ **Microsoft Defender Office 365 Plan 2** หรือ Office 365 Enterprise **E5** Attack Defender **จะไม่** รวมอยู่ใน Microsoft Defender Office 365 Plan 1, Office 365 Enterprise E3 หรือMicrosoft 365 Apps for businessการสมัครใช้งานใดๆ

- บัญชีที่คุณใช้เพื่อเปิดใช้การโจมตีที่จําเป็นต้องมีผู้ดูแลระบบส่วนกลางหรือสิทธิ์ผู้ดูแลระบบความปลอดภัยและการรับรองความถูกต้องโดยใช้หลายปัจจัย (MFA) For more information about Attack Attack Attack requirements, [see this](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)topic .

- สิ่งสําคัญที่ควรทราบ **เกี่ยวกับสถานการณ์โจมตีของ Brute Force** Password:

  - ถ้าบัญชีเป้าหมายเปิดใช้งาน MFA และรหัสผ่านคาดเดาไม่ถูกต้อง บัญชีจะไม่แสดงเป็นบัญชีที่ถูกละเมิด (ปัจจัยการรับรองความถูกต้องที่สองจะไม่สมบูรณ์)

  - ไฟล์รหัสผ่านไม่สามารถมีขนาดใหญ่กว่า 10 MB ได้ ใช้รหัสผ่านหนึ่งรหัสผ่านต่อบรรทัด และใส่บรรทัดว่าง (อักขระขึ้นบรรทัดใหม่) หลังรหัสผ่านสุดท้ายในรายการ

- สิ่งสําคัญที่ต้องทราบเกี่ยวกับ **ฟิชชิ่งของ Phishing** แนบการสถานการณ์:

  - ตามการออกแบบ คุณไม่สามารถใส่ URL เซิร์ฟเวอร์การเข้าสู่ระบบฟิชชิ่ง

  - ถ้าผู้รับใช้ [Add-in เปิดใช้งานข้อความ](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) รายงาน เพื่อรายงานข้อความเป็นฟิชชิ่ง คุณอาจไม่ได้รับการแจ้งเตือนข้อความนั้น (เนื่องจากนี่คือการโจมตีที่จําเป็น)

- รายงาน: หลังจากการโจมตีที่จําเป็นเสร็จสมบูรณ์ คุณสามารถ **คลิก รายละเอียด** การโจมตี เพื่อดูรายงานได้

- ดูคําแนะนําโดยละเอียดและฟีเจอร์ใหม่ใน Attackขออภัย[ให้ดู Attackขออภัยใน Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
