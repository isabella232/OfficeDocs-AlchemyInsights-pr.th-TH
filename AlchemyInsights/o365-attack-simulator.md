---
title: จําลองการโจมตี 2681 ใน Microsoft 365
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
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713485"
---
# <a name="attack-simulator-in-microsoft-365"></a>จําลองการโจมตีใน Microsoft 365

- คุณหายไปจําลองการโจมตี? จําลองการโจมตีจําเป็นต้องมี**แผนการป้องกันภัยคุกคามขั้นสูงของ Office 365 2 (แผน ATP 2)** หรือ**E5 สําหรับองค์กร Office 365** จําลองการโจมตี**จะไม่**รวมอยู่ในแผนการป้องกันภัยคุกคามขั้นสูงของ Office 365 1 (แผน ATP 1), Office 365 Enterprise E3 หรือแอป Microsoft 365 สําหรับการสมัครใช้งานทางธุรกิจ

- บัญชีที่คุณใช้เพื่อเปิดการโจมตีแบบจําลองสถานการณ์ต้องการสิทธิ์ผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบความปลอดภัยและการตรวจสอบสิทธิ์แบบหลายปัจจัย (MFA) สําหรับข้อมูลเพิ่มเติมเกี่ยวกับข้อกําหนดของตัวจําลองการโจมตี ให้ดูที่[หัวข้อนี้](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin)

- สิ่งสําคัญที่ควรทราบเกี่ยวกับการจําลองแบบ**โจมตี Brute Force:**

  - หากบัญชีเป้าหมายมีการเปิดใช้งาน MFA และรหัสผ่านถูกเดาอย่างถูกต้อง

  - แฟ้มรหัสผ่านต้องไม่มากกว่า 10 MB ใช้รหัสผ่านหนึ่งต่อบรรทัด และรวมบรรทัดว่าง (carriage return) หลังรหัสผ่านล่าสุดในรายการ

- สิ่งสําคัญที่ควรทราบเกี่ยวกับการจําลองการ**หลอกลวงหอก**แนบ:

  - การออกแบบคุณไม่สามารถให้ค่าที่กําหนดเองสําหรับ**URL เซิร์ฟเวอร์การเข้าสู่ระบบฟิชชิ่ง**

  - ถ้าผู้รับใช้[Add-in ข้อความรายงาน](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)การเปิดใช้งานเพื่อรายงานข้อความเป็นฟิชชิ่ง คุณอาจไม่ได้รับการแจ้งเตือนสําหรับข้อความ (เนื่องจากนี่เป็นการโจมตีแบบจําลอง)

- รายงาน: หลังจากการโจมตีแบบจําลองสถานการณ์เสร็จสมบูรณ์แล้ว**Attack Details**

- สําหรับคําแนะนําโดยละเอียดและคุณลักษณะใหม่ๆ ใน Simulator การโจมตี ให้ดูที่[เครื่องมือจําลองการโจมตีใน Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
