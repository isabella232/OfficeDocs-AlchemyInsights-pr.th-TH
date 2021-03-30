---
title: Single-Signเปิดบนอุปกรณ์ที่เข้าร่วมของ Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405663"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>การเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวบนอุปกรณ์ที่เข้าร่วมของ Azure Active Directory

ถ้าคุณมีสภาพแวดล้อม Active Directory (AD) ภายในองค์กร และคุณต้องการเข้าร่วมคอมพิวเตอร์ที่เข้าร่วมโดเมน AD กับ Azure AD คุณสามารถทํางานนี้ให้เสร็จได้โดยการเข้าร่วม Azure AD แบบไฮบริด [วิธีการ: วางแผนการปรับใช้การเข้าร่วม Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) แบบไฮบริดจะให้คุณมีขั้นตอนที่เกี่ยวข้องเพื่อปรับใช้การเข้าร่วม Azure AD แบบไฮบริดในสภาพแวดล้อมของคุณ

[กําหนดค่าอุปกรณ์ที่เข้าร่วมของ Azure AD Single-Signภายในองค์กรโดยใช้ Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**ปัญหาโทเค็นรีเฟรชหลัก (PRT)** โทเค็นรีเฟรชหลัก (PRT) คือสิ่งประดิษฐ์หลักของการรับรองความถูกต้อง Azure AD บน Windows 10, Windows Server 2016 และเวอร์ชันที่ใหม่กว่า, iOS และอุปกรณ์ Android ซึ่งเป็นโทเค็นเว็บ JSON (JWT) ที่ออกให้กับนายหน้าโทเค็นของบริษัทแรกใน Microsoft เพื่อเปิดใช้งานการลงชื่อเข้าระบบครั้งเดียว (SSO) ในแอปพลิเคชันที่ใช้บนอุปกรณ์เหล่านั้น [โทเค็นรีเฟรชหลักคืออะไร เราจะ](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)ให้รายละเอียดเกี่ยวกับวิธีการออก ใช้ และป้องกัน PRT บนอุปกรณ์ Windows 10

**WamDefaultSet: YES และ AzureADPrt: YES** เขตข้อมูลเหล่านี้ระบุว่าผู้ใช้ได้รับการรับรองความถูกต้องไปยัง Azure AD เรียบร้อยแล้วหรือไม่เมื่อลงชื่อเข้าใช้อุปกรณ์ ถ้าค่าเป็น **NO** อาจเป็นเพราะ:

- คีย์ที่เก็บข้อมูลที่ไม่ดีใน TPM ที่เชื่อมโยงกับอุปกรณ์เมื่อลงทะเบียน (ตรวจสอบ KeySignTest ขณะที่เรียกใช้สิทธิ์ผู้ดูแล)
- รหัสการเข้าสู่ระบบอื่น
- ไม่พบพร็อกซี HTTP

แก้ไขปัญหาอุปกรณ์โดยใช้สั่ง dsregcmd - [สถานะ SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
