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
ms.openlocfilehash: 627048f21eb931188dfebd3f4177be2bbd65c71e26ab2d0e302f5ab49e9fbc53
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900091"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>ให้ผู้ใช้ซิงค์บัญชีส่วนบุคคลกับบัญชีที่Microsoft Edge

ตรวจสอบให้แน่ใจว่าคุณมีคุณสมบัติตรงตามเกณฑ์เหล่านี้:

- เปิดใช้งานการโรมมิ่งสถานะองค์กรAzure Active Directoryศูนย์การจัดการระบบซึ่งต้องมีการสมัครใช้งาน Azure Active Directory Premium Enterprise Mobility + Security (EMS) ดูข้อมูลเพิ่มเติมได้ที่ เปิดใช้งานการ[โรมมิ่งสถานะองค์กรใน Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-enable)
- ตรงตามเกณฑ์ใดเกณฑ์หนึ่งหรือทั้งสองข้อต่อไปนี้
    - เปิดใช้งานบริการ Azure Information Protection กับผู้เช่าของคุณ โปรดดูรายละเอียดที่[เปิดใช้งาน Azure Rights Management protection ศูนย์การจัดการ Microsoft 365](https://docs.microsoft.com/azure/information-protection/activate-office365)
    - ฟีเจอร์Azure Active Directoryการใช้งานข้ามเขตรัฐขององค์กร (ESR) จะเปิดใช้งานให้กับผู้ใช้หรือผู้เช่า For more info, see [What is enterprise state roaming?](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-overview).

ถ้าทั้ง AIP และ ESR ถูกปิดใช้งาน ข้อความแสดงข้อผิดพลาดจะแจ้งผู้ใช้ว่าการซิงค์ไม่พร้อมใช้งานกับบัญชีผู้ใช้ของพวกเขา
