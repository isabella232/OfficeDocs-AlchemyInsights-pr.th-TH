---
title: 2681 โจมตีจําลองใน Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506757"
---
# <a name="attack-simulator-in-microsoft-365"></a>จําลองการโจมตีใน Microsoft 365

- คุณหายไปโจมตีจําลอง? โปรแกรมจําลองการโจมตีจําเป็นต้องมี**แผนการป้องกันภัยคุกคามขั้นสูง 365 Office 2 (ATP Plan 2)** หรือ**Office 365 Enterprise E5** ตัวจําลองการโจมตี**ไม่ได้**รวมอยู่ในแผนการป้องกันภัยคุกคามขั้นสูงของ Office 365 1 (แผน ATP 1), Office 365 Enterprise E3 หรือแอป Microsoft 365 สําหรับการบอกรับเป็นสมาชิกทางธุรกิจ

- บัญชีที่คุณใช้เพื่อเปิดใช้การโจมตีจําลองต้องการสิทธิ์ระดับผู้ดูแลหรือผู้ดูแลความปลอดภัยส่วนกลางและการรับรองความถูกต้องด้วยหลายปัจจัย (MFA) สําหรับข้อมูลเพิ่มเติมเกี่ยวกับข้อกําหนดของ Attack Simulator โปรดดู[หัวข้อนี้](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- สิ่งสําคัญที่ควรรู้เกี่ยวกับ**การจําลองการโจมตี Brute Force Password:**

  - หากบัญชีเป้าหมายเปิดใช้งาน MFA และเดารหัสผ่านถูกต้องบัญชีจะไม่แสดงเป็น compromised (ปัจจัยการตรวจสอบที่สองจะไม่สมบูรณ์)

  - แฟ้มรหัสผ่านไม่สามารถมีขนาดใหญ่กว่า 10 เมกะไบต์ได้ ใช้รหัสผ่านหนึ่งครั้งต่อบรรทัด และรวมบรรทัดว่าง (กลับค่าขนส่ง) หลังจากรหัสผ่านล่าสุดในรายการ

- สิ่งสําคัญที่ต้องทราบเกี่ยวกับการจําลอง**การแนบฟิชชิ่ง Spear:**

  - โดยการออกแบบ คุณไม่สามารถกําหนดค่าที่กําหนดเองสําหรับ**URL ของเซิร์ฟเวอร์การเข้าสู่ระบบฟิชชิ่ง**

  - ถ้าผู้รับใช้[add-in การเปิดใช้งานข้อความรายงาน](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)เพื่อรายงานข้อความว่าเป็นฟิชชิ่ง คุณอาจไม่ได้รับข้อความแจ้งเตือน (เนื่องจากเป็นการโจมตีจําลอง)

- รายงาน: หลังจากการโจมตีจําลองเสร็จสมบูรณ์แล้ว**Attack Details**

- สําหรับคําแนะนําโดยละเอียดและคุณลักษณะใหม่ในการโจมตีจําลอง ดู[จําลองการโจมตี ใน Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
