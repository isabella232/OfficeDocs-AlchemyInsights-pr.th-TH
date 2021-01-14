---
title: ปัญหาเกี่ยวกับการรวม SSO อย่างราบรื่นกับแอปภายในองค์กรของฉัน
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868769"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>ปัญหาเกี่ยวกับการรวม SSO อย่างราบรื่นกับแอปภายในองค์กรของฉัน

เมื่อต้องการแก้ไขปัญหาเกี่ยวกับการรวม SSO ที่ไม่ราบรื่นกับแอปพลิเคชันภายในองค์กรให้ทำดังต่อไปนี้:

**ขั้นตอนที่แนะนำ**

1. เมื่อต้องการกำหนดค่า **แอปพลิเคชันภายในองค์กร** สำหรับการ **ลงชื่อเข้าใช้ครั้งเดียวผ่านทางพร็อกซีแอปพลิเคชัน** ให้ดู [รหัสผ่านลิ่วสำหรับการลงชื่อเข้าใช้ครั้งเดียวด้วยพร็อกซีแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **การแก้ไขปัญหาเกี่ยวกับพร็อกซีของแอปพลิเคชัน**: เราขอแนะนำให้คุณเริ่มต้นด้วยการตรวจทานการแก้ไขปัญหาการแก้ไขปัญหาการ [เชื่อมต่อพร็อกซีของแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)การตรวจสอบความถูกต้อง ถ้าคุณยังคงมีปัญหาในการเชื่อมต่อกับแอปพลิเคชันให้ทำตามขั้นตอนการแก้ไขปัญหาในการ [แก้ปัญหาแอปพลิเคชันพร็อกซีของแอปพลิเค](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)ชัน คุณสามารถ [ระบุปัญหา CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ได้โดยใช้เครื่องมือตรวจแก้จุดบกพร่องของเบราว์เซอร์ต่อไปนี้:
    1. เปิดใช้งานเบราว์เซอร์แล้วเรียกดูเว็บแอป
    1. กด **F12** เพื่อเปิดคอนโซลการตรวจแก้จุดบกพร่อง
    1. ลองสร้างทรานแซคชันใหม่และรีวิวข้อความของคอนโซล การละเมิด CORS สร้างข้อผิดพลาดของคอนโซลเกี่ยวกับจุดเริ่มต้น
    1. ปัญหา CORS บางอย่างไม่สามารถแก้ไขได้เช่นเมื่อแอปของคุณเปลี่ยนเส้นทางไปยัง login.microsoftonline.com เพื่อรับรองความถูกต้องและโทเค็นการเข้าถึงหมดอายุ การโทร CORS จะล้มเหลว วิธีแก้ไขปัญหาชั่วคราวสำหรับสถานการณ์สมมตินี้คือการขยายอายุการใช้งานของโทเค็นการเข้าถึงเพื่อป้องกันไม่ให้มีการหมดอายุระหว่างเซสชันของผู้ใช้ สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการทำสิ่งนี้ให้ดูที่ค่าที่ได้จากการกำหนดค่าของ[โทเค็นใน Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**เอกสารที่แนะนำ**

- [วิธีการกำหนดค่าการลงชื่อเข้าระบบครั้งเดียวไปยังแอปพลิเคชันพร็อกซีของแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [การลงชื่อเข้าใช้ครั้งเดียวของ SAML สำหรับแอปพลิเคชันภายในองค์กรที่มีพร็อกซีแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [ทำความเข้าใจและแก้ไขปัญหาพร็อกซีแอปพลิเคชัน active Directory ของ Azure CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [แก้ไขปัญหาการกำหนดค่าการมอบหมาย Kerberos ที่จำกัดสำหรับพร็อกซีแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)