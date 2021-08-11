---
title: การกําหนดค่าพร็อกซีแอป
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
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951584"
---
# <a name="app-proxy-configuration"></a>การกําหนดค่าพร็อกซีแอป

1. เมื่อต้องการเข้าใจวิธีกําหนดค่าแอปพลิเคชันพร็อกซีแอปพลิเคชันภายใน Azure AD เพื่อแสดงแอปพลิเคชันภายในองค์กรของคุณไปยังระบบคลาวด์ ให้ดู วิธีการกําหนด [ค่าแอปพลิเคชันพร็อกซี](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)แอปพลิเคชัน
2. การลงชื่อเข้าระบบครั้งเดียว (SSO) ช่วยให้ผู้ใช้ของคุณสามารถเข้าถึงแอปพลิเคชันโดยไม่ต้องรับรองความถูกต้องหลายครั้ง ซึ่งอนุญาตให้มีการรับรองความถูกต้องเดียวเกิดขึ้นในระบบคลาวด์ เทียบกับ Azure Active Directory และอนุญาตให้บริการหรือตัวเชื่อมต่อเลียนแบบผู้ใช้เพื่อเสร็จสิ้นความท้าทายการรับรองความถูกต้องเพิ่มเติมจากแอปพลิเคชัน เมื่อต้องการเรียนรู้เพิ่มเติม [ให้ดู วิธีการกําหนดค่าการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวไปยังแอปพลิเคชันพร็อกซี](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)แอปพลิเคชัน
3. ใช้ [บทความนี้](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) เพื่อแก้ไขปัญหาทั่วไปที่บุคคลต้องเผชิญเมื่อสร้างแอปพลิเคชันพร็อกซีแอปพลิเคชันใหม่
4. ถ้าคุณมีปัญหาในการตั้งค่าการรับรองความถูกต้อง Back-end ให้กับแอปพลิเคชันของคุณ คุณอาจต้อง แก้ไขปัญหาการกําหนดค่าการมอบสิทธิ์แบบมีข้อกําหนดของ [Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) สําหรับพร็อกซีแอปพลิเคชัน หรือให้ปฏิบัติตามแนวทางในการกําหนดค่าแอปพลิเคชันด้วย [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) เพื่อแก้ไขปัญหาของคุณ
