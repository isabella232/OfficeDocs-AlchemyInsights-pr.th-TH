---
title: การแจ้งเตือน AAD Connect
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
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037234"
---
# <a name="notification-aad-connect"></a>การแจ้งเตือน AAD Connect

- ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดําเนินการ ผู้ดูแลระบบส่วนกลางมีสิทธิ์เข้าถึงได้ตามค่าเริ่มต้น นอกจากนี้ คุณสามารถใช้การควบคุมการเข้าถึง [ตามบทบาทเพื่อมอบ](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) สิทธิ์การลงทะเบียนให้กับผู้สนับสนุน
- ตรวจสอบให้แน่ใจว่าจุดสิ้นสุดที่กําหนดเปิดใช้งาน และไม่ถูกบล็อกเนื่องจากไฟร์วอลล์ For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- การลงทะเบียนอาจล้มเหลวเนื่องจากการสื่อสารขาออกต้องผ่านการตรวจสอบ SSL โดยชั้นเครือข่าย
- ตรวจสอบให้แน่ใจว่าคุณได้ตรวจสอบการตั้งค่าการแจ้งเตือนของ Azure AD Connect Health และตรวจสอบการตั้งค่าของคุณ เมื่อต้องการเข้าใจวิธีกําหนดค่าการตั้งค่าการแจ้งเตือนการแจ้งเตือนของ Azure AD Connect Health ให้ดู [คู่มือ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)นี้
- เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับรายงานการซิงค์ AAD Connect Health และวิธีดาวน์โหลด ให้ดู [รายงานการซิงโครไนซ์ระดับ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)วัตถุ

เมื่อต้องการแก้ไขปัญหาการแจ้งเตือนสถานภาพของ AAD Connect ให้ปฏิบัติตามคู่มือการแก้ไขปัญหาเกี่ยวกับการแจ้งเตือนความสมบูรณ์ของข้อมูล [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) และถามบ่อย ให้ดูข้อถามการติดตั้ง [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)ทั่วไป
