---
title: แก้ไขปัญหาใบรับรองการเซ็นชื่อ SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: fb043122edf5f99325f0403810eb0dc119d254e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314439"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>แก้ไขปัญหาใบรับรองการเซ็นชื่อ SAML

เมื่อต้องการแก้ไขปัญหาใบรับรองการเซ็นชื่อ SAML ให้ปฏิบัติตามขั้นตอนที่แนะนําต่อไปนี้:

1. เมื่อคุณเพิ่มแอปพลิเคชันขององค์กรที่สนับสนุน SSO แล้ว Azure จะสร้างใบรับรองซึ่งเรียกว่าใบรับรอง[การเซ็นชื่อ SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) ใบรับรองนี้มีวันหมดอายุ 3 ปี เมื่อต้องการเปลี่ยนวันหมดอายุของใบรับรองของคุณ ให้ดู [ปรับแต่งวันหมดอายุของใบรับรองการติดต่อกับภายนอกของคุณ และย้อนกลับไปยังใบรับรอง](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)ใหม่
2. Azure จะใช้ใบรับรองนี้ในการเซ็นชื่อโทเค็น SAML ที่แอปพลิเคชันร้องขอและส่งไปยังแอปพลิเคชันเพื่อ SSO ที่สําเร็จ เมื่อต้องการเสร็จสิ้น ให้ดาวน์โหลดใบรับรองจากพอร์ทัล Azure และส่งใบรับรองนั้นไปยังผู้ออกแอปพลิเคชันเพื่อเสร็จสิ้นกระบวนการ SSO

หลังจากกระบวนการนี้เสร็จสมบูรณ์ แอปพลิเคชันของคุณจะเชื่อถือใบรับรองนี้และโทเค็น SAML ทั้งหมดที่เซ็นชื่อโดยใบรับรองนี้จะถูกยอมรับโดยแอปพลิเคชัน

3. ถ้าใบรับรองนี้หมดอายุ ให้สร้างใบรับรองใหม่ อัปเดตใบรับรองนั้นไปยังผู้ขายแอปพลิเคชัน แล้วเปิดใช้งานบนด้าน Azure For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

**หมายเหตุ**: ถ้าใบรับรองหมดอายุ ผู้ใช้จะไม่ถูกบล็อก

4. [เพิ่มที่อยู่อีเมลเพื่อให้ได้รับ](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) การแจ้งเตือนก่อนที่ใบรับรองปัจจุบันจะหมดอายุ

**หมายเหตุ**: ขั้นตอนที่ 4 เป็นตัวเลือกเพิ่มเติม

5. เปลี่ยนตัวเลือกการเซ็นชื่อใบรับรอง SAML ของแอปพลิเคชันและอัลกอริทึมการเซ็นชื่อใบรับรอง For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

