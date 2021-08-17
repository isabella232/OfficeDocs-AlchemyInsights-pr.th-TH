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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084365"
---
# <a name="sso-connection-issues"></a>ปัญหาการเชื่อมต่อ SSO

1. Follow the [Quickstart: Configure properties for an application](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) guide to configure your application.
2. ขึ้นอยู่กับแอปพลิเคชันและตัวเลือก [การลงชื่อเข้าระบบครั้งเดียว](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) ที่คุณเลือก ให้ปฏิบัติตามแนวทางที่เหมาะสมด้านล่าง:
    - เมื่อต้องการกําหนด **ค่าแอปพลิเคชันภายในองค์กร** ของการเข้าสู่ระบบ **โดยลงชื่อเข้าใช้** ครั้งเดียวแบบ SAML ให้ดูที่ [การลงชื่อเข้าระบบครั้งเดียว SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)ของแอปพลิเคชันภายในองค์กรที่มี พร็อกซีแอปพลิเคชัน
    - เมื่อต้องการกําหนด **ค่าแอปพลิเคชันระบบคลาวด์****ให้การลงชื่อเข้าระบบครั้งเดียว** ที่ใช้รหัสผ่าน [ให้ดูที่ กําหนดค่าการลงชื่อเข้าระบบครั้งเดียวของ](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)รหัสผ่าน
    - เมื่อต้องการกําหนด **ค่าแอปพลิเคชันภายในองค์กรการ****ลงชื่อเข้าระบบครั้งเดียวผ่านพร็อกซี** แอปพลิเคชัน ให้ดูที่ [ชุดรหัสผ่านแบบลงชื่อเข้าใช้ครั้งเดียวด้วยพร็อกซี](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)แอปพลิเคชัน
3. **การแก้ไขปัญหาพร็อกซีแอปพลิเคชัน**: เราขอแนะนนะให้คุณเริ่มต้นด้วยการตรวจทานโฟลว์ [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)การแก้ไขปัญหา ปัญหาจุดบกพร่องของตัวเชื่อมต่อพร็อกซีแอปพลิเคชัน เพื่อตรวจสอบว่าตัวเชื่อมต่อพร็อกซีแอปพลิเคชันถูกกําหนดค่าอย่างถูกต้องหรือไม่ ถ้าคุณยังคงมีปัญหาในการเชื่อมต่อกับแอปพลิเคชัน ให้ปฏิบัติตามขั้นตอนการแก้ไขปัญหาใน ปัญหา[แอปพลิเคชัน Debug Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) คุณสามารถระบุ [ปัญหา CORS โดยใช้](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) เครื่องมือแก้ไขจุดบกพร่องของเบราว์เซอร์:
    - เปิดใช้เบราว์เซอร์และเรียกดูเว็บแอป
    - กด **F12** เพื่อแสดงคอนโซลแก้ไขจุดบกพร่อง
    - พยายามสร้างทรานแซคชันขึ้นและตรวจสอบข้อความคอนโซล การละเมิด CORS สร้างข้อผิดพลาดของคอนโซลเกี่ยวกับที่มา
    - ปัญหา CORS บางอย่างไม่สามารถแก้ไขได้ เช่น เมื่อแอปของคุณเปลี่ยนเส้นทาง login.microsoft.com เพื่อรับรองความถูกต้อง และโทเค็นการเข้าถึงจะหมดอายุ การโทรผ่าน CORS จะล้มเหลว วิธีแก้ไขปัญหาชั่วคราวของสถานการณ์สมมตินี้คือการขยายอายุการใช้งานโทเค็นการเข้าถึง เพื่อป้องกันไม่ให้หมดอายุระหว่างเซสชันของผู้ใช้ For more information about how to do this, see [Configurable token lifetimes in แพลตฟอร์มข้อมูลประจําตัวของ Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **การแก้ไขปัญหาการ** ลงชื่อเข้าระบบครั้งเดียวแบบ SAML : เราขอแนะให้ตรวจสอบ ปัญหาในการลงชื่อเข้าใช้แอปที่กําหนดค่าการลงชื่อเข้าระบบครั้งเดียวแบบ [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)เพื่อค้นหาวิธีแก้ไขปัญหาที่คุณมีแนวโน้มที่จะพบมากที่สุด
5. **การแก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียว** โดยใช้รหัสผ่าน: เราขอแนะนนะให้ตรวจสอบ แก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียวโดยใช้รหัสผ่านใน [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)เพื่อค้นหาวิธีแก้ไขปัญหาที่คุณมีแนวโน้มที่จะพบมากที่สุด
6. For connection issues while using a VPN, see [How to use single sign on (SSO) over VPN and Wi-Fi connections](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
