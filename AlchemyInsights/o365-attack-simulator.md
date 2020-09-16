---
title: ๒๖๘๑จำลองการโจมตีใน Microsoft ๓๖๕
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759238"
---
# <a name="attack-simulator-in-microsoft-365"></a>จำลองการโจมตีใน Microsoft ๓๖๕

- คุณไม่พบการจำลองการโจมตีใช่ไหม จำลองการโจมตีจำเป็นต้องมี**Office ๓๖๕การป้องกันภัยคุกคามขั้นสูงแผน 2 (ATP Plan 2)** หรือ**Office ๓๖๕ Enterprise E5** การโจมตีของการโจมตีจะ **ไม่** รวมอยู่ใน Office ๓๖๕การป้องกันภัยคุกคามขั้นสูงสำหรับแผน 1 (ATP Plan 1), Office ๓๖๕ Enterprise E3 หรือการสมัครใช้งาน Microsoft ๓๖๕ Apps for business

- บัญชีผู้ใช้ที่คุณใช้เพื่อเปิดใช้งานการโจมตีแบบจำลองจำเป็นต้องมีสิทธิ์ผู้ดูแลระบบส่วนกลางหรือสิทธิ์ผู้ดูแลระบบความปลอดภัยและการรับรองความถูกต้องแบบหลายปัจจัย (MFA) สำหรับข้อมูลเพิ่มเติมเกี่ยวกับความต้องการของการโจมตีของ Simulator ให้ดู[หัวข้อนี้](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- สิ่งสำคัญที่ควรทราบเกี่ยวกับการจำลองการโจมตีของ **รหัสผ่าน** ที่รุนแรง:

  - ถ้าบัญชีผู้ใช้เป้าหมายมีการเปิดใช้งาน MFA และรหัสผ่านถูกคาดเดาได้อย่างถูกต้องบัญชีผู้ใช้จะไม่แสดงเป็นที่ถูกบุกรุก (ปัจจัยการรับรองความถูกต้องที่สองจะไม่สมบูรณ์)

  - ไฟล์รหัสผ่านจะต้องมีขนาดใหญ่กว่า10เมกะไบต์ ใช้รหัสผ่านหนึ่งบรรทัดต่อหนึ่งบรรทัดและรวมบรรทัดว่าง (ส่งกลับค่าขนส่ง) หลังจากรหัสผ่านสุดท้ายในรายการ

- สิ่งสำคัญที่ควรทราบเกี่ยวกับสถานการณ์จำลองที่แนบมาของการ **ฟิชชิ่งของหอก** :

  - ตามการออกแบบคุณจะไม่สามารถใส่ค่าที่กำหนดเองสำหรับ **URL ของเซิร์ฟเวอร์การเข้าสู่ระบบฟิชชิ่ง**ได้

  - ถ้าผู้รับใช้ [Add-in ข้อความรายงาน](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) เพื่อรายงานข้อความเป็นฟิชชิ่งคุณอาจไม่ได้รับการแจ้งเตือนสำหรับข้อความ (เนื่องจากเป็นการโจมตีแบบจำลอง)

- รายงาน: หลังจากการโจมตีแบบจำลองเสร็จสมบูรณ์แล้วคุณสามารถคลิก **รายละเอียดการโจมตี** เพื่อดูรายงานได้

- สำหรับคำแนะนำโดยละเอียดและฟีเจอร์ใหม่ในการโจมตีจำลองให้ดู[ที่จำลองการโจมตีใน Microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
