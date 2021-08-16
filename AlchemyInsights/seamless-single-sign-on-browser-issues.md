---
title: แก้ไขปัญหาเบราว์เซอร์การเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) อย่างราบรื่น
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9377"
ms.openlocfilehash: f8617c15072f70778f7f4b151e75ffce4749f89ffa2b4d91730937c26aaeabbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074309"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-browser-issues"></a>แก้ไขปัญหาเบราว์เซอร์การเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) อย่างราบรื่น

ผู้ใช้ส่วนใหญ่สามารถแก้ไขปัญหาเบราว์เซอร์ SSO ได้อย่างราบรื่นได้โดยใช้ขั้นตอนด้านล่าง:

1. ตรวจสอบให้แน่ใจว่าเบราว์เซอร์ของคุณทันสมัย
2. ลบคุกกี้จากเบราว์เซอร์ของคุณเพื่อเอาเซสชัน SSO ที่ไม่ถูกต้องออก และลองเข้าสู่ระบบอีกครั้ง
3. ลองเข้าสู่ระบบโดยใช้เบราว์เซอร์อื่น

**ปัญหาเบราว์เซอร์ที่ทราบแล้ว**

- SSO อย่างราบรื่นไม่ใช้งานในโหมดการเรียกดูส่วนบุคคลบน Firefox
- SSO อย่างราบรื่นไม่ใช้งานใน Internet Explorer เมื่อเปิดโหมดที่ได้รับการป้องกันขั้นสูง
- SSO อย่างราบรื่นไม่ใช้งานในโหมดการเรียกดูส่วนบุคคลบนMicrosoft Edge (แบบดั้งเดิม)
- SSO อย่างราบรื่นไม่ใช้งานบนเบราว์เซอร์บนอุปกรณ์เคลื่อนที่บน iOS และ Android

SSO อย่างราบรื่น สนับสนุนเวอร์ชันถัดไปMicrosoft EdgeโดยยึดตามChromium และใช้งานได้ในโหมด InPrivate และ Guest ตามการออกแบบ

**การปรึกษา**

เมื่อต้องการร้องขอฟีเจอร์หรือถามข้อถามทางเทคนิคเกี่ยวกับ SSO อย่างราบรื่น ให้ดู การถาม&[A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html)
