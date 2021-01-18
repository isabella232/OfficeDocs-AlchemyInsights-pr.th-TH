---
title: การกำหนดค่าพร็อกซีของแอป
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885530"
---
# <a name="app-proxy-configuration"></a>การกำหนดค่าพร็อกซีของแอป

1. เมื่อต้องการทำความเข้าใจเกี่ยวกับวิธีการกำหนดค่าแอปพลิเคชันพร็อกซีของแอปพลิเคชันภายใน Azure AD เพื่อแสดงแอปพลิเคชันภายในองค์กรของคุณไปยัง cloud ให้ดูที่[วิธีการกำหนดค่าแอปพลิเคชันพร็อกซี](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)
2. การลงชื่อเข้าระบบครั้งเดียว (SSO) ช่วยให้ผู้ใช้ของคุณสามารถเข้าถึงแอปพลิเคชันได้โดยไม่มีการรับรองความถูกต้องหลายครั้ง จะอนุญาตให้มีการรับรองความถูกต้องเดียวที่จะเกิดขึ้นในระบบคลาวด์จาก Azure Active directory และอนุญาตให้บริการหรือตัวเชื่อมต่อเพื่อ impersonate ผู้ใช้ให้ทำการท้าทายการรับรองความถูกต้องเพิ่มเติมใดๆเพิ่มเติมจากแอปพลิเคชัน เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่ [วิธีการกำหนดค่าการลงชื่อเข้าระบบครั้งเดียวไปยังแอปพลิเคชันพร็อกซีแอปพลิ](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)เคชัน
3. ใช้ [บทความนี้](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) เพื่อแก้ไขปัญหาทั่วไปที่คนหน้าเมื่อสร้างแอปพลิเคชันพร็อกซีของแอปพลิเคชันใหม่
4. ถ้าคุณกำลังมีปัญหาในการตั้งค่าการรับรองความถูกต้องของการสิ้นสุดหลังไปยังแอปพลิเคชันของคุณคุณอาจต้องการแก้ไขปัญหาการ[กำหนดค่าการมอบสิทธิ์ kerberos ที่จำกัดสำหรับพร็อกซีแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to)หรือทำตามคำแนะนำเกี่ยวกับการ[กำหนดค่าแอปพลิเคชันด้วย PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to)
