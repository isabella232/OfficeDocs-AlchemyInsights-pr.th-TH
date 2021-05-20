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
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539699"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>ปัญหาในการติดตั้ง Microsoft Defender บน Mac หรือ Linux

**Mac**

- ตรวจสอบให้แน่ใจว่าเป็นไปตามความต้องการของระบบก่อนที่จะMicrosoft Defender ATP for Mac ดูข้อมูลเพิ่มเติมได้ที่ วิธีการติดตั้ง[อุปกรณ์ Microsoft Defender ATP for](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)Mac  
- ตรวจทานข้อมูลในไฟล์: "/Library/Logs/Microsoft/mdatp/install.log"

**Linux**

- ตรวจสอบให้แน่ใจว่าเป็นไปตามความต้องการของระบบก่อนที่จะติดตั้งMicrosoft Defender ATP For Linux For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- เมื่อต้องการตรวจสอบว่าบริการ MDATP ใช้งานอยู่ ให้ดู [การติดตั้ง](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)ล้มเหลว  
    เมื่อต้องการแก้ไขปัญหาถ้าบริการไม่ได้เรียกใช้อยู่ ให้ดู [ขั้นตอนการแก้ไขปัญหาถ้าบริการ mdatp ไม่ได้](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)เรียกใช้อยู่
- For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **หมายเหตุ** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).