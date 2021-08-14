---
title: มีปัญหาในการตั้งค่ารหัสผ่านใหม่แบบบริการตนเอง (SSPR) ใช่หรือไม่
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002464"
- "7663"
ms.openlocfilehash: bd76ae6b2ce140fd8feb490a5fffe1baa36598e7650107f176baec30d71b8628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945869"
---
# <a name="having-self-service-password-reset-sspr-problems"></a>มีปัญหาในการตั้งค่ารหัสผ่านใหม่แบบบริการตนเอง (SSPR) ใช่หรือไม่

ปัญหาทั่วไปในการรีเซ็ตรหัสผ่านด้วยตนเอง (SSPR) ในสภาพแวดล้อมระบบคลาวด์แบบไฮบริดและภายในองค์กร คือ:

- [ไม่ได้เปิดใช้งาน Writeback ของรหัสผ่าน SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)
- [ไม่ได้มอบหมายสิทธิ์การใช้งาน Azure AD Premium](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing)
- [ปัญหาหรือเชื่อมต่อระบบเครือข่ายของ](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors)Azure [](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-connectivity) AD
- [วิธีการรับรองความถูกต้อง SSPR ที่ไม่ได้ลงทะเบียน](https://mysignins.microsoft.com/security-info)
- [สถานการณ์ writeback ที่ไม่ได้รับการสนับสนุน เช่น ศูนย์](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-writeback#unsupported-writeback-operations)การเขียนการจัดการ Microsoft 365หรือผู้ดูแลระบบโดยใช้ SSPR


สำหรับข้อมูลเพิ่มเติม ให้ดู:

- [แก้ไขปัญหาการตั้งค่ารหัสผ่านใหม่แบบบริการตนเอง](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr)
- [แก้ไขปัญหา Writeback การตั้งค่ารหัสผ่านใหม่แบบบริการตนเองในAzure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)
