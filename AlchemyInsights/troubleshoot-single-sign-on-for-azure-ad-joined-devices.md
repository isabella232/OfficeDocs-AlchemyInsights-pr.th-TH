---
title: แก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียวบนอุปกรณ์ที่เข้าร่วมของ Azure AD
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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037335"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>แก้ไขปัญหาการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวบนอุปกรณ์ที่เข้าร่วมของ Azure AD

ถ้าคุณมีสภาพแวดล้อม Active Directory (AD) ภายในองค์กร และคุณต้องการเข้าร่วมคอมพิวเตอร์ที่เข้าร่วมโดเมน AD กับ Azure AD คุณสามารถทํางานนี้ได้โดยการเข้าร่วม Azure AD แบบไฮบริด [วิธีการ: วางแผนการปรับใช้การเข้าร่วม Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) แบบไฮบริดจะให้คุณมีขั้นตอนที่เกี่ยวข้องเพื่อปรับใช้การเข้าร่วม Azure AD แบบไฮบริดในสภาพแวดล้อมของคุณ

ดูข้อมูลเพิ่มเติมในการกําหนด [ค่าอุปกรณ์ที่เข้าร่วมของ Azure AD](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)Single-Signเปิดใช้งาน Windows Hello for Business

**ปัญหาโทเค็นรีเฟรชหลัก (PRT)**

โทเค็นรีเฟรชหลัก (PRT) คือสิ่งประดิษฐ์หลักของการรับรองความถูกต้อง Azure AD บนอุปกรณ์ Windows 10, Windows Server 2016 และเวอร์ชันที่ใหม่กว่า, iOS และ Android ซึ่งเป็นโทเค็นเว็บ JSON (JWT) ที่ออกให้กับนายหน้าโทเค็นของบริษัทแรกใน Microsoft เพื่อเปิดใช้งานการลงชื่อเข้าระบบครั้งเดียว (SSO) ในแอปพลิเคชันที่ใช้บนอุปกรณ์เหล่านั้น For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

**WamDefaultSet: YES และ AzureADPrt: YES**

เขตข้อมูลเหล่านี้ระบุว่าผู้ใช้ได้รับการรับรองความถูกต้องไปยัง Azure AD เรียบร้อยแล้วหรือไม่เมื่อลงชื่อเข้าใช้อุปกรณ์ ถ้าค่าเป็น **NO** อาจเป็นเพราะ:

- คีย์ที่เก็บข้อมูลที่ไม่ดีใน TPM ที่เชื่อมโยงกับอุปกรณ์เมื่อลงทะเบียน (ตรวจสอบ KeySignTest ขณะที่เรียกใช้สิทธิ์ผู้ดูแล)
- รหัสการเข้าสู่ระบบอื่น
- ไม่พบพร็อกซี HTTP

เมื่อต้องการแก้ไขปัญหาอุปกรณ์โดยใช้สั่ง dsregcmd ให้ดู[สถานะ SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
