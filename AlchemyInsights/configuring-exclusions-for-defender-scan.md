---
title: การกําหนดค่าข้อยกเว้นของ Microsoft Defender ATP สแกน
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
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "50714354"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a>การกําหนดค่าข้อยกเว้นของ Microsoft Defender ATP สแกน

โดยทั่วไปแล้ว คุณสามารถยกเว้นส่วนขยายของไฟล์และโฟลเดอร์บางรายการจากการสแกน MICROSOFT Defender ATP คุณยังสามารถกําหนดค่าการยกเว้นไฟล์ที่เปิดโดยกระบวนการบางอย่างได้ For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and Configure [exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .

เมื่อต้องการกําหนดค่าข้อยกเว้นของ **Windows Server 2016 และ 2019** ให้ดู การกําหนดค่าการยกเว้น [โปรแกรมป้องกันไวรัสของ Microsoft Defender บน Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)

**Mac**

For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).

**หมายเหตุ** คุณสามารถตรวจสอบรายการยกเว้นโดยใช้ไฟล์ทดสอบ EICAR ได้ For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file). 

**Linux**

For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).

**หมายเหตุ** คุณสามารถตรวจสอบรายการยกเว้นโดยใช้ไฟล์ทดสอบ EICAR ได้ For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file). 