---
title: Single-Signเปิดขึ้นAzure Active Directoryอุปกรณ์ที่เข้าร่วม
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
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050029"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>การเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวAzure Active Directoryที่เข้าร่วม

ถ้าคุณมีสภาพแวดล้อม Active Directory (AD) ภายในองค์กร และคุณต้องการเข้าร่วมคอมพิวเตอร์ที่เข้าร่วมโดเมน AD ของคุณไปยัง Azure AD คุณสามารถทํางานนี้ให้เสร็จได้โดยการเข้าร่วม Azure AD แบบไฮบริด [วิธีการ: วางแผนการปรับใช้การเข้าร่วมAzure Active Directoryแบบไฮบริด](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan)ของคุณมีขั้นตอนที่เกี่ยวข้องเพื่อปรับใช้การเข้าร่วม Azure AD แบบไฮบริดในสภาพแวดล้อมของคุณ

[กําหนดค่าอุปกรณ์ที่เข้าร่วมของ Azure AD Single-Signเปิด การใช้งาน Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**ปัญหาโทเค็นรีเฟรชหลัก (PRT)** โทเค็นรีเฟรชหลัก (PRT) คืออาร์แฟกต์หลักของการรับรองความถูกต้อง Azure AD Windows 10, Windows Server 2016 และอุปกรณ์ iOS และ Android เวอร์ชันที่ใหม่กว่า It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices. [ใน โทเค็นรีเฟรชหลักคืออะไร](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)เราจะให้รายละเอียดเกี่ยวกับวิธีการออก ใช้ และป้องกัน PRT Windows 10บนอุปกรณ์ของคุณ

**WamDefaultSet: YES และ AzureADPrt: YES** เขตข้อมูลเหล่านี้ระบุว่าผู้ใช้ได้รับการรับรองความถูกต้อง Azure AD เมื่อลงชื่อเข้าใช้อุปกรณ์เรียบร้อยแล้วหรือไม่ ถ้าค่าเป็น **ไม่ใช่** อาจเป็นเพราะ:

- คีย์ที่เก็บข้อมูลที่ไม่ดีใน TPM ที่เชื่อมโยงกับอุปกรณ์เมื่อลงทะเบียน (ตรวจสอบ KeySignTest ขณะที่เรียกใช้สิทธิ์ผู้ดูแล)
- รหัสการเข้าสู่ระบบอื่น
- ไม่พบพร็อกซี HTTP

แก้ไขปัญหาอุปกรณ์โดยใช้สั่ง dsregcmd - [สถานะ SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
