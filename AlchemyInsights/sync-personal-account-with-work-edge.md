---
title: ให้ผู้ใช้ซิงค์บัญชีส่วนบุคคลกับบัญชีที่Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813408"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>ให้ผู้ใช้ซิงค์บัญชีส่วนบุคคลกับบัญชีที่Microsoft Edge

ตรวจสอบให้แน่ใจว่าคุณมีคุณสมบัติตรงตามเกณฑ์เหล่านี้:

- เปิดใช้งานการโรมมิ่งสถานะองค์กรAzure Active Directoryศูนย์การจัดการระบบจดหมาย ซึ่งAzure Active Directory Premium Enterprise Mobility + Security (EMS) ดูข้อมูลเพิ่มเติมได้ที่ เปิดใช้งานการ[โรมมิ่งสถานะองค์กรใน Azure Active Directory](/azure/active-directory/devices/enterprise-state-roaming-enable)
- ตรงตามเกณฑ์ใดเกณฑ์หนึ่งหรือทั้งสองข้อต่อไปนี้
    - บริการ Azure Information Protection ถูกเปิดใช้งานให้ผู้เช่าของคุณ For details, see [Activate Azure Rights Management protection from the ศูนย์การจัดการ Microsoft 365](/azure/information-protection/activate-office365).
    - ฟีเจอร์ Azure Active Directoryการใช้งานข้ามเขตรัฐขององค์กร (ESR) จะเปิดใช้งานให้กับผู้ใช้หรือผู้เช่า For more info, see [What is enterprise state roaming?](/azure/active-directory/devices/enterprise-state-roaming-overview).

ถ้าทั้ง AIP และ ESR ถูกปิดใช้งาน ข้อความแสดงข้อผิดพลาดจะแจ้งผู้ใช้ว่าการซิงค์ไม่พร้อมใช้งานกับบัญชีผู้ใช้ของพวกเขา
