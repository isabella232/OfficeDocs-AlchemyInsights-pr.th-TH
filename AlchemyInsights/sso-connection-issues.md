---
title: ปัญหาการเชื่อมต่อ SSO
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
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935205"
---
# <a name="sso-connection-issues"></a>ปัญหาการเชื่อมต่อ SSO

1. Follow the [Quickstart: Configure properties for an application](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) guide to configure your application.
2. ขึ้นอยู่กับแอปพลิเคชันและ [ตัวเลือกการลงชื่อเข้าระบบ](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) ครั้งเดียวที่คุณเลือก ให้ปฏิบัติตามแนวทางที่เหมาะสมทางด้านล่าง:
    - เมื่อต้องการกําหนด **ค่าแอปพลิเคชันภายในองค์กร** ของการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวแบบ **SAML** ให้ดูที่ การลงชื่อเข้าระบบครั้งเดียว SAML ของแอปพลิเคชันภายใน [องค์กรที่มีพร็อกซี](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)แอปพลิเคชัน
    - เมื่อต้องการกําหนด **ค่าแอปพลิเคชันระบบคลาวด์****ให้การลงชื่อเข้าระบบครั้งเดียว** ที่ยึดตามรหัสผ่าน [ให้ดูที่ กําหนดค่าการลงชื่อเข้าระบบครั้งเดียวของรหัสผ่าน](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - เมื่อต้องการกําหนด **ค่าแอปพลิเคชันภายในองค์กรการ****ลงชื่อเข้าระบบครั้งเดียวผ่านพร็อกซี** แอปพลิเคชัน ให้ดูที่ [Password vaulting for single sign-on ด้วยพร็อกซี](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)แอปพลิเคชัน
3. **การแก้ไขปัญหาพร็อกซีแอปพลิเคชัน**: เราขอแนะนนะให้คุณเริ่มต้นด้วยการตรวจทานขั้นตอนการแก้ไขปัญหา ปัญหา Debug [Application Proxy Connector](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)เพื่อระบุว่าตัวเชื่อมต่อพร็อกซีแอปพลิเคชันถูกกําหนดค่าอย่างถูกต้องหรือไม่ ถ้าคุณยังคงมีปัญหาในการเชื่อมต่อกับแอปพลิเคชัน ให้ปฏิบัติตามขั้นตอนการแก้ไขปัญหาในปัญหา [แอปพลิเคชันพร็อกซีแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)แก้จุดบกพร่อง คุณสามารถระบุ [ปัญหา CORS โดยใช้](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) เครื่องมือแก้จุดบกพร่องของเบราว์เซอร์:
    - เปิดใช้เบราว์เซอร์และเรียกดูเว็บแอป
    - กด **F12** เพื่อให้คอนโซลแก้ไขจุดบกพร่องแสดงขึ้น
    - พยายามสร้างทรานแซคชันขึ้นและตรวจสอบข้อความคอนโซล การละเมิด CORS สร้างข้อผิดพลาดของคอนโซลเกี่ยวกับที่มา
    - ปัญหาบางอย่างของ CORS ไม่สามารถแก้ไขได้ เช่น เมื่อแอปของคุณเปลี่ยนเส้นทางlogin.microsoft.comเพื่อรับรองความถูกต้อง และโทเค็นการเข้าถึงหมดอายุ การโทรผ่าน CORS จะล้มเหลว วิธีแก้ไขปัญหาชั่วคราวในสถานการณ์สมมตินี้คือการยืดอายุอายุการใช้งานของโทเค็นการเข้าถึง เพื่อป้องกันไม่ให้หมดอายุระหว่างเซสชันของผู้ใช้ For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **การแก้ไขปัญหาการ** ลงชื่อเข้าระบบครั้งเดียวแบบ SAML : เราขอแนะนนะให้ตรวจสอบปัญหาในการลงชื่อเข้าใช้แอปที่กําหนดค่าโดยลงชื่อเข้าใช้ครั้งเดียวแบบ [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)เพื่อค้นหาวิธีแก้ไขปัญหาที่คุณมีแนวโน้มที่จะพบ
5. **การแก้ไขปัญหาการลงชื่อเข้าระบบ** ครั้งเดียวโดยใช้รหัสผ่าน : เราขอแนะนนะให้ตรวจสอบการแก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียวโดยใช้รหัสผ่านใน [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)เพื่อค้นหาวิธีแก้ไขปัญหาที่คุณมีแนวโน้มที่จะพบมากที่สุด
6. For connection issues while using a VPN, see [how to use single sign on (SSO) over VPN and Wi-Fi connections](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
