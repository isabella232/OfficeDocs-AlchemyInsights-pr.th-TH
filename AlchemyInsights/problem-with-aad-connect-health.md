---
title: ปัญหากับ AAD Connect Health
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
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483122"
---
# <a name="problem-with-aad-connect-health"></a>ปัญหากับ AAD Connect Health

- ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดําเนินการ ผู้ดูแลระบบส่วนกลางมีสิทธิ์เข้าถึงได้ตามค่าเริ่มต้น นอกจากนี้ คุณสามารถใช้การควบคุมการเข้าถึง [ตามบทบาทเพื่อมอบ](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) สิทธิ์การลงทะเบียนให้กับผู้สนับสนุน
- ตรวจสอบให้แน่ใจว่าจุดสิ้นสุดที่กําหนดเปิดใช้งาน และไม่ถูกบล็อกเนื่องจากไฟร์วอลล์ For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- การลงทะเบียนอาจล้มเหลวเนื่องจากการสื่อสารขาออกต้องผ่านการตรวจสอบ SSL โดยชั้นเครือข่าย
- ตรวจสอบให้แน่ใจว่าคุณได้ตรวจสอบการตั้งค่าการแจ้งเตือนของ Azure AD Connect Health แล้ว โปรดตรวจสอบการตั้งค่าของคุณ คู่มือ [นี้](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) สามารถช่วยให้คุณเข้าใจวิธีการกําหนดค่าการตั้งค่าการแจ้งเตือนการแจ้งเตือนสถานภาพ Azure AD Connect
- เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับรายงานการซิงค์ AAD Connect Health และวิธีดาวน์โหลด ให้ดู [รายงานการซิงโครไนซ์ระดับ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)วัตถุ

เมื่อต้องการแก้ไขปัญหาการแจ้งเตือน AAD Connect Health ให้ปฏิบัติตามคู่มือการแก้ไขปัญหาของการแจ้งเตือนความสมบูรณ์ของข้อมูล [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) และถามบ่อย ให้ดูข้อถามการติดตั้ง [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)ทั่วไป
