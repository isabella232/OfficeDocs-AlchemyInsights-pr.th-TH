---
title: การกําหนดค่าการยกเว้นของ Microsoft Defender ATP Scan
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
ms.openlocfilehash: 0b64217062aadea22afe1aa17748a5f38b9f1cd6c59adc54345afe3c6f12bdc2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900351"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a>การกําหนดค่าการยกเว้นของ Microsoft Defender ATP Scan

โดยทั่วไปแล้ว คุณสามารถยกเว้นส่วนขยายของไฟล์และโฟลเดอร์บางรายการจากการสแกน Microsoft Defender ATP คุณยังสามารถกําหนดค่าการยกเว้นไฟล์ที่เปิดโดยกระบวนการบางอย่างได้ For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and Configure [exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .

เมื่อต้องการกําหนดค่าการยกเว้น **Windows Server 2016 และ 2019** ให้ดูที่ กําหนดค่าโปรแกรมป้องกันไวรัสของ Microsoft Defender [แยกออกWindowsเซิร์ฟเวอร์](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)

**Mac**

For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).

**หมายเหตุ** คุณยังสามารถตรวจสอบรายการยกเว้นโดยใช้ไฟล์ทดสอบ EICAR ได้ For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file). 

**Linux**

For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).

**หมายเหตุ** คุณยังสามารถตรวจสอบรายการยกเว้นโดยใช้ไฟล์ทดสอบ EICAR ได้ For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file). 