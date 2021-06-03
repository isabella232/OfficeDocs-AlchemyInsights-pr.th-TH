---
title: จุดสิ้นสุด DLP ไม่ได้ปรับใช้กับอุปกรณ์ของผู้ใช้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731870"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>จุดสิ้นสุด DLP ไม่ได้ปรับใช้กับอุปกรณ์ของผู้ใช้

ถ้าการตั้งค่า การป้องกันการสูญหายของข้อมูลจุดสิ้นสุด (DLP) ไม่ได้ใช้กับอุปกรณ์ของผู้ใช้ ให้ยืนยันว่าคุณตรงตามข้อต้องการเหล่านี้:

- Windows 10 x64 รุ่น 1809 หรือใหม่กว่าได้รับการติดตั้งบนอุปกรณ์แล้ว
- ไคลเอ็นต์ป้องกันมัลแวร์เวอร์ชัน 4.18.2009.7 หรือใหม่กว่าได้รับการติดตั้งแล้ว
- อุปกรณ์คือ **หนึ่งใน** อุปกรณ์ต่อไปนี้:
    
    - Azure Active Directory (Azure AD) เข้าร่วม
    - Azure AD แบบไฮบริดที่เข้าร่วม
    - AAD ที่ลงทะเบียน

- เมื่อต้องการบังคับใช้การบังคับใช้นโยบาย ตรวจสอบให้แน่ใจว่าเบราว์เซอร์ Microsoft Chromium Edge ถูกติดตั้งบนอุปกรณ์จุดสิ้นสุด

For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).