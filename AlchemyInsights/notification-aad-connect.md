---
title: การแจ้งเตือน AAD เชื่อมต่อ
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
- "9003245"
- "9326"
ms.openlocfilehash: b8713700ee4fc8863a269c99b92954e1df45e1e647c491fb9b439ab83c49f2ff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097325"
---
# <a name="notification-aad-connect"></a>การแจ้งเตือน AAD เชื่อมต่อ

- ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดําเนินการ ผู้ดูแลระบบส่วนกลางจะมีสิทธิ์เข้าถึงตามค่าเริ่มต้น นอกจากนี้ คุณสามารถใช้การควบคุมการเข้าถึง [ตามบทบาทเพื่อ](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) มอบสิทธิ์การลงทะเบียนให้กับผู้สนับสนุน
- ตรวจสอบให้แน่ใจว่าเปิดใช้งานจุดสิ้นสุดที่กําหนดและไม่บล็อกเนื่องจากไฟร์วอลล์ โปรดดูรายละเอียดที่[ข้อกฎหมาย](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- การลงทะเบียนอาจล้มเหลวเนื่องจากการสื่อสารขาออกถูกต้องผ่านการตรวจสอบ SSL โดยชั้นเครือข่าย
- ตรวจสอบให้แน่ใจว่าคุณได้ตรวจสอบการตั้งค่าการแจ้งเตือนของ Azure AD เชื่อมต่อสถานภาพและตรวจสอบการตั้งค่าของคุณ เมื่อต้องการเข้าใจวิธีกําหนดค่าการตั้งค่าการแจ้งเตือนของ Azure AD เชื่อมต่อสถานภาพการแจ้งเตือน ให้ดู[คู่มือ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)นี้
- เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับรายงานเชื่อมต่อ AAD และวิธีดาวน์โหลด ให้ดู รายงานการ[ซิงโครไนซ์ระดับ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)วัตถุ

เมื่อต้องการแก้ไขปัญหา AAD เชื่อมต่อการแจ้งเตือนสถานภาพ ให้ปฏิบัติตามคู่มือการแก้ไขปัญหาของ[AAD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness)เชื่อมต่อการแจ้งเตือนความใหม่ของข้อมูลสถานภาพและถามที่ถามบ่อย ให้ดู ปัญหาการติดตั้งสถานภาพ เชื่อมต่อ[AAD](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)ทั่วไป
