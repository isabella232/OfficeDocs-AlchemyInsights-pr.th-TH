---
title: แก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่น (SSO) โดยใช้รหัสผ่าน
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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714889"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>แก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่น (SSO) โดยใช้รหัสผ่าน

เมื่อต้องการเรียนรู้พื้นฐานของ SSO ที่ใช้รหัสผ่าน ให้ดูการรับรองความถูก[ต้องโดยใช้รหัสผ่านด้วย Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**กําหนดค่า SSO ที่ใช้รหัสผ่าน**

1. [กําหนดค่าการลงชื่อเข้าระบบครั้งเดียว](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) โดยใช้รหัสผ่าน - บทความนี้มีรายละเอียดเพิ่มเติมเกี่ยวกับตัวเลือก SSO ที่ใช้รหัสผ่าน ถ้าแอปพลิเคชันที่คุณเพิ่มต้องการการกําหนดค่าแบบกําหนดเองและคุณต้องใช้ SSO ที่ใช้รหัสผ่าน บทความนี้มีไว้เพื่อคุณ
2. [กําหนดค่าการลงชื่อเข้าระบบครั้งเดียวโดยใช้รหัสผ่านของแอปภายในเครื่อง](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - พร็อกซีแอปพลิเคชันสนับสนุนโหมดการลงชื่อเข้าระบบครั้งเดียวหลายโหมด การลงชื่อเข้าใช้ด้วยรหัสผ่านมีไว้เพื่อแอปพลิเคชันที่ใช้การรวมกันของชื่อผู้ใช้/รหัสผ่านเพื่อการรับรองความถูกต้อง เมื่อคุณกําหนดค่าการลงชื่อเข้าใช้ด้วยรหัสผ่านของแอปพลิเคชันของคุณ ผู้ใช้ของคุณจะต้องลงชื่อเข้าใช้แอปพลิเคชันภายในองค์กรหนึ่งครั้ง หลังจากนั้น Azure Active Directory จะจัดเก็บข้อมูลการลงชื่อเข้าใช้และมอบข้อมูลนั้นไปยังแอปพลิเคชันโดยอัตโนมัติเมื่อผู้ใช้ของคุณเข้าถึงจากระยะไกล
    - คุณควรเผยแพร่และทดสอบแอปของคุณด้วยพร็อกซีแอปพลิเคชันแล้ว ถ้าไม่ ให้ปฏิบัติตามขั้นตอนใน [ประกาศแอปพลิเคชันโดยใช้พร็อกซี](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) แอปพลิเคชัน Azure AD จากนั้นให้กําหนดค่า SSO ที่ยึดตามรหัสผ่านของคุณต่อไป

เมื่อต้องการแก้ไขปัญหา SSO ที่ยึดตามรหัสผ่าน ให้ดู [แก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียวโดยใช้รหัสผ่านใน Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
