---
title: แก้ไขปัญหาการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) โดยใช้รหัสผ่าน
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
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972843"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>แก้ไขปัญหาการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) โดยใช้รหัสผ่าน

เมื่อต้องการเรียนรู้พื้นฐานของ SSO ที่ใช้รหัสผ่าน ให้ดู การรับรองความถูก[ต้องโดยใช้รหัสผ่านAzure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)รหัสผ่าน

**การกําหนดค่า SSO ที่ใช้รหัสผ่าน**

1. [กําหนดค่าการลงชื่อเข้าระบบครั้งเดียว](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) โดยใช้รหัสผ่าน - บทความนี้ใส่รายละเอียดเพิ่มเติมเกี่ยวกับตัวเลือก SSO ที่ยึดตามรหัสผ่าน ถ้าแอปพลิเคชันที่คุณเพิ่มต้องการการกําหนดค่าแบบกําหนดเอง และคุณต้องใช้ SSO ที่ใช้รหัสผ่าน บทความนี้มีไว้เพื่อคุณ
2. [กําหนดค่าการลงชื่อเข้าระบบครั้งเดียวบนรหัสผ่านของแอปในเครื่อง](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - พร็อกซีแอปพลิเคชันสนับสนุนโหมดการลงชื่อเข้าระบบครั้งเดียวหลายโหมด การลงชื่อเข้าใช้ด้วยรหัสผ่านมีไว้เพื่อแอปพลิเคชันที่ใช้การผสมชื่อผู้ใช้/รหัสผ่านเพื่อการรับรองความถูกต้อง เมื่อคุณกําหนดค่าการลงชื่อเข้าใช้ด้วยรหัสผ่านของแอปพลิเคชันของคุณ ผู้ใช้ของคุณจะต้องลงชื่อเข้าใช้แอปพลิเคชันภายในองค์กรหนึ่งครั้ง หลังจากนั้น Azure Active Directoryเก็บข้อมูลการลงชื่อเข้าใช้และมอบข้อมูลนั้นให้กับแอปพลิเคชันโดยอัตโนมัติเมื่อผู้ใช้ของคุณเข้าถึงจากระยะไกล
    - คุณควรเผยแพร่และทดสอบแอปของคุณด้วยพร็อกซีแอปพลิเคชันแล้ว ถ้าไม่ ให้ปฏิบัติตามขั้นตอนใน [เผยแพร่แอปพลิเคชันโดยใช้พร็อกซี](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) แอปพลิเคชัน Azure AD จากนั้นให้กําหนดค่า SSO ที่ใช้รหัสผ่านต่อในแอปภายในเครื่อง

เมื่อต้องการแก้ไขปัญหา SSO ที่ใช้รหัสผ่าน ให้ดู [แก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียวโดยใช้รหัสผ่านใน Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
