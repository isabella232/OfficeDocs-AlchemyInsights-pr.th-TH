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
ms.openlocfilehash: 507dc5a3bdc5f1bc27cf12865daf98df6c702827
ms.sourcegitcommit: f835aa80f2d85e9c0549be9395110377dba50f3d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695344"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-browser-issues"></a>แก้ไขปัญหาเบราว์เซอร์การเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) อย่างราบรื่น

ผู้ใช้ส่วนใหญ่สามารถแก้ไขปัญหาเบราว์เซอร์ SSO อย่างราบรื่นได้โดยใช้ขั้นตอนด้านล่าง:

1. ตรวจสอบให้แน่ใจว่าเบราว์เซอร์ของคุณทันสมัย
2. ลบคุกกี้จากเบราว์เซอร์เพื่อเอาเซสชัน SSO ที่ไม่ถูกต้องออก แล้วลองเข้าสู่ระบบอีกครั้ง
3. ลองเข้าสู่ระบบโดยใช้เบราว์เซอร์อื่น

**ปัญหาที่ทราบเกี่ยวกับเบราว์เซอร์**

- SSO อย่างราบรื่นไม่ใช้งานในโหมดการเรียกดูส่วนบุคคลบน Firefox
- SSO อย่างราบรื่นไม่ใช้งานใน Internet Explorer เมื่อเปิดโหมดที่ได้รับการป้องกันขั้นสูง
- SSO อย่างราบรื่นไม่ใช้งานในโหมดการเรียกดูส่วนบุคคลบน Microsoft Edge (แบบดั้งเดิม)
- SSO อย่างราบรื่นไม่ใช้งานบนเบราว์เซอร์อุปกรณ์เคลื่อนที่บน iOS และ Android

SSO อย่างราบรื่นสนับสนุน Microsoft Edge เวอร์ชันถัดไปโดยยึดตาม Chromium และใช้งานในโหมด InPrivate และโหมด Guest ตามการออกแบบ

**การปรึกษา**

เมื่อต้องการร้องขอฟีเจอร์หรือถามข้อสงสัยทางเทคนิคเกี่ยวกับ SSO อย่างราบรื่น ให้ดูการถามตอบของ [Microsoft&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html)
