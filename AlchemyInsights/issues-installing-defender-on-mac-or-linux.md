---
title: ปัญหาในการติดตั้ง Microsoft Defender บน Mac หรือ Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "50714318"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>ปัญหาในการติดตั้ง Microsoft Defender บน Mac หรือ Linux

**Mac**

- ตรวจสอบให้แน่ใจว่าเป็นไปตามความต้องการของระบบก่อนที่จะติดตั้ง Microsoft Defender ATP for Mac For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- ตรวจทานข้อมูลในไฟล์: "/Library/Logs/Microsoft/mdatp/install.log"

**Linux**

- ตรวจสอบให้แน่ใจว่าเป็นไปตามความต้องการของระบบก่อนที่จะติดตั้ง Microsoft Defender ATP for Linux For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- เมื่อต้องการตรวจสอบว่าบริการ MDATP เรียกใช้อยู่ หรือไม่ [ให้ดูที่ การติดตั้ง](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)ล้มเหลว  
    เมื่อต้องการแก้ไขปัญหาถ้าบริการไม่ได้เรียกใช้อยู่ ให้ดู[ขั้นตอนการแก้ไขปัญหาถ้าบริการ mdatp ไม่ได้ใช้งาน](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **หมายเหตุ** ดูรายการระบบไฟล์ที่สนับสนุนกิจกรรมการเข้าถึงได้ที่ [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)