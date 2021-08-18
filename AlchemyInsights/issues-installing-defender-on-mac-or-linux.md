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
ms.openlocfilehash: defc11265caf371ce0a62a10a5de1d8ff88a8e11
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325268"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>ปัญหาในการติดตั้ง Microsoft Defender บน Mac หรือ Linux

**Mac**

- ตรวจสอบให้แน่ใจว่าเป็นไปตามความต้องการของระบบก่อนที่จะติดตั้ง Microsoft Defender ATP for Mac ดูข้อมูลเพิ่มเติมได้ที่ วิธีการติดตั้ง[Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- ตรวจทานข้อมูลในไฟล์: "/Library/Logs/Microsoft/mdatp/install.log"

**Linux**

- ตรวจสอบให้แน่ใจว่าเป็นไปตามความต้องการของระบบก่อนที่จะติดตั้ง Microsoft Defender ATP for Linux For more info, see [How to install MDATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- เมื่อต้องการตรวจสอบว่าบริการ MDATP ใช้งานอยู่ ให้ดู [การติดตั้ง](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)ล้มเหลว  
    เมื่อต้องการแก้ไขปัญหาถ้าบริการไม่ได้เรียกใช้อยู่ ให้ดู [ขั้นตอนการแก้ไขปัญหาถ้าบริการ mdatp ไม่ได้](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)เรียกใช้อยู่
- For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **หมายเหตุ** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).