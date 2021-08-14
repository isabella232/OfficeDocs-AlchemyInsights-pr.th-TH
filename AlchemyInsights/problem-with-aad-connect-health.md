---
title: ปัญหากับ AAD เชื่อมต่อ Health
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
- "9004649"
- "8427"
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923771"
---
# <a name="problem-with-aad-connect-health"></a>ปัญหากับ AAD เชื่อมต่อ Health

- ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดําเนินการ ผู้ดูแลระบบส่วนกลางจะมีสิทธิ์เข้าถึงตามค่าเริ่มต้น นอกจากนี้ คุณสามารถใช้การควบคุมการเข้าถึง [ตามบทบาทเพื่อ](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) มอบสิทธิ์การลงทะเบียนให้กับผู้สนับสนุน
- ตรวจสอบให้แน่ใจว่าเปิดใช้งานจุดสิ้นสุดที่กําหนดและไม่บล็อกเนื่องจากไฟร์วอลล์ โปรดดูรายละเอียดที่[ข้อกฎหมาย](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- การลงทะเบียนอาจล้มเหลวเนื่องจากการสื่อสารขาออกถูกต้องผ่านการตรวจสอบ SSL โดยชั้นเครือข่าย
- ตรวจสอบให้แน่ใจว่าคุณได้ตรวจสอบการตั้งค่าการแจ้งเตือนของ Azure AD เชื่อมต่อสถานภาพ โปรดตรวจสอบการตั้งค่าของคุณ คู่มือ[นี้](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)สามารถช่วยให้คุณเข้าใจวิธีกําหนดค่าการตั้งค่าการแจ้งเตือนของ Azure AD เชื่อมต่อสถานภาพการแจ้งเตือน
- เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับรายงานเชื่อมต่อ AAD และวิธีดาวน์โหลด ให้ดู รายงานการ[ซิงโครไนซ์ระดับ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)วัตถุ

เมื่อต้องการแก้ไขปัญหาการแจ้งเตือนสถานเชื่อมต่อ AAD ให้ปฏิบัติตามคู่มือการแก้ไขปัญหาของ[AAD เชื่อมต่อ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness)การแจ้งเตือนความใหม่ของข้อมูลสถานภาพ และถามบ่อย ให้ดู AAD ทั่วไป เชื่อมต่อ[ถามเกี่ยวกับการติดตั้ง Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
