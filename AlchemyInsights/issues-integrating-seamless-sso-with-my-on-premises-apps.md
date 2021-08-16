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
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028311"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>ปัญหาเกี่ยวกับการรวม SSO อย่างราบรื่นกับแอปภายในองค์กรของฉัน

เมื่อต้องการแก้ไขปัญหาเกี่ยวกับการรวม SSO อย่างราบรื่นกับแอปพลิเคชันในองค์กร ให้ต่อไปนี้:

**ขั้นตอนที่แนะนา**

1. เมื่อต้องการกําหนด **ค่าแอปพลิเคชันภายในองค์กรการ****ลงชื่อเข้าระบบครั้งเดียวผ่านพร็อกซี** แอปพลิเคชัน ให้ดูที่ [ชุดรหัสผ่านแบบลงชื่อเข้าใช้ครั้งเดียวด้วยพร็อกซี](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)แอปพลิเคชัน
1. **การแก้ไขปัญหาพร็อกซีแอปพลิเคชัน**: เราขอแนะนนะให้คุณเริ่มต้นด้วยการตรวจทานโฟลว์การแก้ไขปัญหา [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)ปัญหาจุดบกพร่องของตัวเชื่อมต่อพร็อกซีแอปพลิเคชัน เพื่อตรวจสอบว่าตัวเชื่อมต่อพร็อกซีแอปพลิเคชันถูกกําหนดค่าอย่างถูกต้องหรือไม่ ถ้าคุณยังคงมีปัญหาในการเชื่อมต่อกับแอปพลิเคชัน ให้ปฏิบัติตามขั้นตอนการแก้ไขปัญหาใน แก้จุดบกพร่องปัญหา [แอปพลิเคชันพร็อกซี](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)แอปพลิเคชัน คุณสามารถระบุ [ปัญหา CORS ได้โดยใช้](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) เครื่องมือแก้จุดบกพร่องของเบราว์เซอร์ต่อไปนี้:
    1. เปิดใช้เบราว์เซอร์และเรียกดูเว็บแอป
    1. กด **F12** เพื่อแสดงคอนโซลแก้ไขจุดบกพร่อง
    1. พยายามสร้างทรานแซคชันขึ้นและตรวจสอบข้อความคอนโซล การละเมิด CORS สร้างข้อผิดพลาดของคอนโซลเกี่ยวกับที่มา
    1. ปัญหา CORS บางอย่างไม่สามารถแก้ไขได้ เช่น เมื่อแอปของคุณเปลี่ยนเส้นทาง login.microsoftonline.com เพื่อรับรองความถูกต้อง และโทเค็นการเข้าถึงจะหมดอายุ การโทรผ่าน CORS จะล้มเหลว วิธีแก้ไขปัญหาชั่วคราวของสถานการณ์สมมตินี้คือการขยายอายุการใช้งานโทเค็นการเข้าถึง เพื่อป้องกันไม่ให้หมดอายุระหว่างเซสชันของผู้ใช้ For more information about how to do this, see [Configurable token lifetimes in แพลตฟอร์มข้อมูลประจําตัวของ Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**เอกสารที่แนะนา**

- [วิธีกําหนดค่าการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวในแอปพลิเคชันพร็อกซีแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [การลงชื่อเข้าระบบครั้งเดียว SAML ของแอปพลิเคชันภายในองค์กรด้วยพร็อกซีแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [เข้าใจและแก้ไขปัญหาAzure Active Directoryพร็อกซีแอปพลิเคชัน CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [แก้ไขปัญหาการกําหนดค่าการมอบสิทธิ์แบบมีข้อกําหนดแบบ Kerberos แบบมีข้อกําหนดไว้เพื่อพร็อกซีแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)