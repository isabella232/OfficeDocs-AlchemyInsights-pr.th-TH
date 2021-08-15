---
title: แก้ไขปัญหาการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวบนอุปกรณ์ที่เข้าร่วมของ Azure AD
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
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039265"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>แก้ไขปัญหาการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวบนอุปกรณ์ที่เข้าร่วมของ Azure AD

ถ้าคุณมีสภาพแวดล้อม Active Directory (AD) ภายในองค์กร และคุณต้องการเข้าร่วมคอมพิวเตอร์ที่เข้าร่วมโดเมน AD ของคุณไปยัง Azure AD คุณสามารถทํางานนี้ให้เสร็จได้โดยการเข้าร่วม Azure AD แบบไฮบริด [วิธีการ: วางแผนการปรับใช้การเข้าร่วมAzure Active Directoryแบบไฮบริด](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan)ของคุณมีขั้นตอนที่เกี่ยวข้องเพื่อปรับใช้การเข้าร่วม Azure AD แบบไฮบริดในสภาพแวดล้อมของคุณ

For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**ปัญหาโทเค็นรีเฟรชหลัก (PRT)**

โทเค็นรีเฟรชหลัก (PRT) คืออาร์แฟกต์หลักของการรับรองความถูกต้อง Azure AD Windows 10, Windows Server 2016 และอุปกรณ์ iOS และ Android เวอร์ชันที่ใหม่กว่า It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices. For details on how a PRT is issued, used, and protected on Windows 10 devices, [see What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES และ AzureADPrt: YES**

เขตข้อมูลเหล่านี้ระบุว่าผู้ใช้ได้รับการรับรองความถูกต้อง Azure AD เมื่อลงชื่อเข้าใช้อุปกรณ์เรียบร้อยแล้วหรือไม่ ถ้าค่าเป็น **ไม่ใช่** อาจเป็นเพราะ:

- คีย์ที่เก็บข้อมูลที่ไม่ดีใน TPM ที่เชื่อมโยงกับอุปกรณ์เมื่อลงทะเบียน (ตรวจสอบ KeySignTest ขณะที่เรียกใช้สิทธิ์ผู้ดูแล)
- รหัสการเข้าสู่ระบบอื่น
- ไม่พบพร็อกซี HTTP

เมื่อต้องการแก้ไขปัญหาอุปกรณ์โดยใช้สั่ง dsregcmd ให้ดู[สถานะ SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
